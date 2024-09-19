---
tags:
  - Programming
  - OperatingSystems
---
Files to be used as build inputs do not have to come from the file system.
- The [[Nix]]  language provides [[Nix builtints|built-in]] [[Nix Impurities|impure]] functions to fetch files over the network during the evaluation:
	- `builtin.fetchurl`
	- `builtin.fetchClosure`
	- `builtin.fetchGit`
	- `builtin.fetchTarball`
- There functions evaluate to a file system path in the Nix store
## Example
```
builtins.fetchurl "https://github.com/NixOS/nix/archive/7c3ab5751568a0bc63430b33a5169c5e4784a0ff.tar.gz" 
# evaluates to
# "/nix/store/7dhgs330clj36384akg86140fqkgh8zf-7c3ab5751568a0bc63430b33a5169c5e4784a0ff.tar.gz"

####

builtins.fetchTarball "https://github.com/NixOS/nix/archive/7c3ab5751568a0bc63430b33a5169c5e4784a0ff.tar.gz"
# evaluates to 
# "/nix/store/d59llm96vgis5fy231x6m7nrijs0ww36-source" which is unpacked archive
```
## [Manual](https://nixos.org/manual/nixpkgs/stable/#chap-pkgs-fetchers)
