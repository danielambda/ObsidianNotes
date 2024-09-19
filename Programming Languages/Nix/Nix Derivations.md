---
tags:
  - OperatingSystems
---
Derivations are at the core of both [[Nix]] and the [[Nix]] language:
- The [[Nix]] language is used to describe derivations
- [[Nix]] runs derivations to produce *build results*
- *Build results* can in turn be used as inputs for other derivations
## Declaration
- The [[Nix]] language primitive to declare a derivation is the [[Nix builtints|built-in]] [[Nix Impurities|impure]] functions `derivation`