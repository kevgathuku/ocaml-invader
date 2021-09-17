Alternative to Docker workflow:

On MacOS, ensure `freeglut` is installed:
```sh
brew install freeglut
```

Setup a local opam switch

```sh
opam switch create . ocaml-base-compiler.4.10.2
```

Install the dependencies:
```sh
opam install lablgl obuild core
```

Build the project:
```sh
obuild configure && obuild build
```

And finally run it:
```sh
./ocaml-invader
```
