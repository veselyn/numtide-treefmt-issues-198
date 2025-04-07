```sh
direnv allow || nix develop --impure
cp ignored-file.nix.bak ignored-file.nix
treefmt
diff -s ignored-file.nix.bak ignored-file.nix
```
