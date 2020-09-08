To run:


```
cd lwtlib 
dune build
dune install

cd ../dynlinker
dune exec ./main.exe
```
Entering directory '/home/philip/Documents/ocaml/vibes-foolin'
Done: 0/0 (jobs: 0)Entering directory '/home/philip/Documents/ocaml/vibes-foolin'
Fatal error: exception Dynlink.Error (Dynlink.Cannot_open_dll "Dynlink.Error (Dynlink.Cannot_open_dll \"Failure(\\\"/home/philip/.opam/bappy4/lib/lwt/unix/lwt_unix.cmxs: undefined symbol: caml_mutex_lock\\\")\")")
```

ocaml-base-compiler.4.09.1
lwt :  5.3.0


Adding lwt.unit to the dunefile in dynlinker makes it no longer fail.

Related issue https://github.com/ocaml/dune/issues/2100


