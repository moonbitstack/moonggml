# moonggml

Tensors, the graph you build from them, and the schedule that runs it.

> **Status: planned.** The repository is set up; nothing is
> implemented yet.

Named after [ggml](https://github.com/ggml-org/ggml) and aligned with it over
time; the first version is a slice through the middle rather than all of it.

| Package | What it covers |
|:--|:--|
| `tensor` | Shapes, strides, types, and the quantised formats |
| `graph` | Operations as nodes, and the passes that rewrite them |
| `plan` | Where each intermediate lives, and for how long |
| `run` | The schedule, and the backends it dispatches to |
| `cpu` | The backend that needs nothing |
| `gpu` | The backend over [`moonwgpu`](https://github.com/moonbitstack/moonwgpu) |

## What is deliberately elsewhere

Reading a model file is [`moongguf`](https://github.com/moonbitstack/moongguf)'s;
the device is [`moonwgpu`](https://github.com/moonbitstack/moonwgpu)'s; what a
transformer does with all this is [`mooninfer`](https://github.com/moonbitstack/mooninfer)'s.

## Install

```bash
moon add moonbitstack/moonggml
```

## Licence

Apache-2.0. See [LICENSE](LICENSE).
