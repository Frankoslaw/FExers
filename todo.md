# TODO:

All of this changes are motivated by my personal preferences and probably should not be merged into mainline `Exers` implementation.

## Important:

- [ ] - replace compiler options with string. Do we relly need custom types if most of the compilers have diffrent set of flags. So in my opinion keeping compatibility with C and C++ flags have little to no benefit.
- [ ] - unify compilers, preprocessors and runtimes. They all just consume input and produce output. So there is no reason to create separet implementation for all of them.
- [ ] - add wasmtime support.
- [ ] - diffrentiet, between WASM, WASI and WASIX. They server similar goal, but they should be ussed in diffrent contexts.
- [ ] - add nix support to manage dependencies like wasi-sdk.
- [ ] - scratch3 support.
- [ ] - simplify language compiler struct. I don't think it needs to have over 150 lines.

## Nice to have features:

- [ ] - replace chroot with proot, which does not require escaleted permissions to spawn jail.
- [ ] - Allow for piping stdout of any stage for example runtime as stdin.