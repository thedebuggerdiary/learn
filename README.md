# learn

A hub repository aggregating learning projects for various languages and tools as git submodules.

## Submodules

| Repository | Description |
|---|---|
| [learn_gdb](https://github.com/thedebuggerdiary/learn_gdb) | GDB debugger |
| [learn_android](https://github.com/thedebuggerdiary/learn_android) | Android development |
| [learn_flatbuffer](https://github.com/thedebuggerdiary/learn_flatbuffer) | FlatBuffers serialization |
| [learn_flutter](https://github.com/thedebuggerdiary/learn_flutter) | Flutter UI framework |
| [learn_dart](https://github.com/thedebuggerdiary/learn_dart) | Dart language |
| [learn_typescript](https://github.com/thedebuggerdiary/learn_typescript) | TypeScript |
| [learn_go](https://github.com/thedebuggerdiary/learn_go) | Go language |
| [learn_python](https://github.com/thedebuggerdiary/learn_python) | Python |
| [learn_kotlin](https://github.com/thedebuggerdiary/learn_kotlin) | Kotlin |
| [learn_grpc](https://github.com/thedebuggerdiary/learn_grpc) | gRPC |
| [learn_protobuf](https://github.com/thedebuggerdiary/learn_protobuf) | Protocol Buffers |

## Getting Started

### Clone with all submodules

```bash
git clone --recurse-submodules https://github.com/thedebuggerdiary/learn.git
cd learn
git submodule update --remote   # advance every submodule to the latest tip of main
```

Or using make:

```bash
git clone https://github.com/thedebuggerdiary/learn.git
cd learn
make init
```

### Update all submodules to the latest tip

```bash
git submodule update --remote --merge
```

Or:

```bash
make update
```

## Notes

- Submodules are pinned to a specific commit in this repo. The `branch = main` config in `.gitmodules` tells git which branch to track when you run `--remote`.
- Running `git submodule update --remote` (or `make update`) always pulls the latest `main` commit from each submodule.
- To update a single submodule: `git submodule update --remote learn_go`
