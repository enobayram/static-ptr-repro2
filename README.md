# static-ptr-repro2

This repository contains a repro case for the GHC (8.10.3) bug that sometimes causes linker errors when the StaticPointers language extension is enabled.

In order to reproduce the issue, simple run `stack build` in this repo:

```
$ stack build
...
.../static-ptr-repro2/.stack-work/dist/x86_64-linux/Cabal-3.2.1.0/build/libHSstatic-ptr-repro2-0.1.0.0-AjrmJhPev4OAiYnN9ABj5e.a(Lib.o):ghc_5.c:function hs_spt_init_staticzmptrzmrepro2zm0zi1zi0zi0zmAjrmJhPev4OAiYnN9ABj5e_Lib: error: undefined reference to 'rYB_closure'
```
