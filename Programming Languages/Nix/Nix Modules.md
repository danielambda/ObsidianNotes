---
tags:
  - FunctionalProgramming
  - Programming
  - OperatingSystems
---
## Structure
```
{
	imports = [...];

	options = {...};

	config = {...};
}
```
or the same but as function
```
{ config, options, pkgs, modulesPath }:
{
	#same structure
}
```
- where
- [`config`](https://nixos.wiki/wiki/NixOS:config_argument "NixOS:config argument") is the configuration of the entire system.
- `options` is all option declarations refined with all definition and declaration references.
- `pkgs` is the attribute set extracted from the Nix package collection and enhanced with the `nixpkgs.config` option.
 - `modulesPath` is the location of the `module` directory of NixOS.
## Imports
- Imports are paths to other NixOS modules that should be included in the evaluation of the system configuration. A default set of modules is defined in [`nixos/modules/module-list.nix`](https://github.com/NixOS/nixpkgs/blob/master/nixos/modules/module-list.nix) These don't need to be added in the import list. 
#### Example
```
{
	imports = [
		./otherModule.nix
		/path/to/otherModule.nix
	];

	...
}
```
## Declarations (options)
- To declare option in Options attribute, one has to use `mkOption` function accepting a [[Nix Attribute Set]] with the following attributes:
	- `type` the type of the option. May be omitted. Mostly types are in `lib.types.<type>`
	- `default`
	- `example`
	- `description`
#### Example
```
optionName = mkOption {
	type = lib.types.bool;
	default = false;
	example = true;
	description = "Whatever description you like";
};
```
## Full Example
```
{ lib, pkgs, config, ... }:
with lib;                      
let
  cfg = config.services.hello;
in {
  options.services.hello = {
    enable = mkEnableOption "hello service";
    greeter = mkOption {
      type = types.str;
      default = "world";
    };
  };

  # Define what other settings, services and resources should be active IF
  # a user of this "hello.nix" module ENABLED this module 
  # by setting "services.hello.enable = true;".
  config = mkIf cfg.enable {
    systemd.services.hello = {
      wantedBy = [ "multi-user.target" ];
      serviceConfig.ExecStart = "${pkgs.hello}/bin/hello -g'Hello, ${escapeShellArg cfg.greeter}!'";
    };
  };
}
```