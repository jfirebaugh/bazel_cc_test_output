Bug: `bazel run --script_path=test` fails silently when target uses `shard_count`.

```
$ bazel run --script_path=test test; echo $?
INFO: Analyzed target //:test (0 packages loaded, 0 targets configured).
INFO: Found 1 target...
Target //:test up-to-date:
  bazel-bin/test
INFO: Elapsed time: 0.103s, Critical Path: 0.00s
INFO: 1 process: 1 internal.
INFO: Build completed successfully, 1 total action
INFO: Build completed successfully, 1 total action
2
```
