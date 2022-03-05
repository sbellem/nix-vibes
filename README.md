# nix-vibes
Resources for nix, the package manager

https://nix-community.github.io/awesome-nix/

## Nix Expression Language
* https://learnxinyminutes.com/docs/nix/
* https://nixos.org/manual/nix/stable/#ch-expression-language
* https://nixos.wiki/wiki/Nix_Expression_Language

## Flakes
* https://nixos.wiki/wiki/Flakes
* **excellent**: https://serokell.io/blog/practical-nix-flakes
* https://github.com/colemickens/nixos-flake-example
* https://hoverbear.org/blog/a-flake-for-your-crate/
* https://zimbatm.com/notes/nixflakes
* (perhaps outdated) https://gist.github.com/edolstra/40da6e3a4d4ee8fd019395365e0772e7
* https://blog.ysndr.de/posts/internals/2021-01-01-flake-ification/#creating-a-flake-for-this-blog

## Rust
* Main docs: https://github.com/NixOS/nixpkgs/blob/master/doc/languages-frameworks/rust.section.md

**Overlays**
* https://github.com/oxalica/rust-overlay
* https://github.com/nix-community/fenix

**Tutorials**
* https://www.srid.ca/rust-nix
* https://hadean.com/managing-rust-dependencies-with-nix-part-i/
* https://github.com/Twey/mkRustCrate/

**Cargo subcommands**
* https://github.com/NixOS/nixpkgs/issues/95332

### Examples
* Useful issue for `devShell` (with `flakes`): https://github.com/oxalica/rust-overlay/issues/30
* https://github.com/kamadorueda/alejandra/blob/main/flake.nix
* https://github.com/enarx/enarx/blob/main/flake.nix
* https://github.com/Holo-Host/holo-nixpkgs

### Documentation
For cross-compilation (e.g. custom target) see https://github.com/oxalica/rust-overlay/blob/master/docs/cross_compilation.md.


## Cross-Compilation
* https://nixos.wiki/wiki/Cross_Compiling
* https://matthewbauer.us/blog/beginners-guide-to-cross.html

## Reproducible Builds
* Nix Manual: [Verifying Build Reproducibility](https://nixos.org/manual/nix/stable/advanced-topics/diff-hook.html?highlight=reproducible%20build#verifying-build-reproducibility)

Note that config values (e.g. in `/etc/nix/nix.conf`) can be passed to `nix-build` as in

```console
nix-build --option sandbox true --option enforce-determinism true --option repeat 3
```

* [Is NixOS Reproducible?](https://r13y.com/) -- See last section "How can I test my patches?" about the trick of using `nix-build --check`

* [Reproducible Builds: Nix vs Docker](https://discourse.nixos.org/t/resources-that-explains-nix-vs-docker-for-reproducible-builds/9508)

* Could [`flakes`](https://nixos.wiki/wiki/Flakes) help? https://discourse.nixos.org/t/to-flake-or-not-to-flake/10047/4
* [Will Nix overtake Docker?](https://blog.replit.com/nix-vs-docker)
* https://news.ycombinator.com/item?id=29387137
* https://news.ycombinator.com/item?id=24981633
* https://serokell.io/blog/what-is-nix
* https://plurrrr.com/archive/2021/11/30.html
* https://chameth.com/reproducible-builds-docker-images/

