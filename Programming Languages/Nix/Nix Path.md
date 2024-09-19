---
tags:
  - FunctionalProgramming
  - Programming
  - OperatingSystems
---
## There is a Path [[Data Type]] in [[Nix]]
## Syntax
```
/etc/nixos/configurations.nix
./.
../.
./assets/hyprland-anime-girl.jpg
```
## String Interpolation Nuance 
- Whenever a file system path is used in string interpolation, the contents of that file are copied to a special location in the file system, the [[Nix]] store , as a [[Nix Impurities|side effect]]
- The evaluated string then contains the [[Nix]] store path assigned to that file.
#### Example
```bash
echo 123 > data
```
```
"${./data}" # evaluates to "/nix/store/h1qj5h5n05b5dl5q4nldrqq8mdg7dhqk-data"
```
##### For directories
- the same thing happens: The entire directory (including nested files and directories) is copied to the Nix store, and the evaluated string becomes the Nix store path of the directory.