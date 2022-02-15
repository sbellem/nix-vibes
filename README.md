# nix-vibes
Resources for nix, the package manager


## Reproducible Builds
* Nix Manual: [Verifying Build Reproducibility](https://nixos.org/manual/nix/stable/advanced-topics/diff-hook.html?highlight=reproducible%20build#verifying-build-reproducibility)

Note that config values (e.g. in `/etc/nix/nix.conf`) can be passed to `nix-build` as in

```console
nix-build --option sandbox true --option enforce-determinism true --option repeat 3
```

* [Is NixOS Reproducible?](https://r13y.com/) -- See last section "How can I test my patches?" about the trick of using `nix-build --check`

* [Reproducible Builds: Nix vs Docker](https://discourse.nixos.org/t/resources-that-explains-nix-vs-docker-for-reproducible-builds/9508)

* Could [`flakes`](https://nixos.wiki/wiki/Flakes) help? https://discourse.nixos.org/t/to-flake-or-not-to-flake/10047/4
