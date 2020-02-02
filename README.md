# manual-stg-experiment

Manually constructed STG programs compiled with the standard GHC codegen backend.

### Build

```
stack setup
stack build
```

### Usage

```
stack ghci StgSample.hs
```

Run a sample in GHCi. i.e.

```
*StgSample> sampleADT2
```

It will generate an executable named `a.out` also will generate the intermediate output files (`out.ll`, `out.s`, `out.o`).

### Why?

This experiment suggests that GHC codegen and RTS can be used as generic compiler backend for strict and lazy functional languages.  
The samples show various use cases i.e. (de)construction of (un)boxed tuples and (un)lifted ADTs and using FFI.
