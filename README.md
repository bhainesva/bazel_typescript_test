## VSCODE/Bazel Import Error Repro

1. Clone this repo. Open in vscode.
2. See that the import of `"bazel_typescript_test/src/lib"` from `src/index.ts` works fine / can be clicked through.
3. Run `bazel build //src:ts_lib`.
4. See that editor now complains the same import in `src/index.ts` is invalid.
5. Run `bazel clean` and see that the editor is happy with the import again