# Ichnaea
Ichnaea is a lightweight interrupt-based tracer for dynamic memory objects. Ichnaea traces rich context information without sacrificing performance.
---
## Features
- Very-low overhead when objects aren’t touched
- Traces Kernel Writes
- Traces multithreaded workloads
- Rich context per access (who wrote, where, what, when)
- Works with `LD_PRELOAD` and simple header annotations
- Fuzzer-friendly alternative to heavyweight tools like Pin or Valgrind
## Repo
The main repo lives [here.](https://github.com/IchnaeaTracer/Ichnaea) (Updates coming Soon)
## Quick Start
```bash
# Build
make
# Run program under tracer
LD_PRELOAD=./libichnaea.so ./your_program
```
