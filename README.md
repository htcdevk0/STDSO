# stdso

`stdso` is a single-header C++ utility for POSIX dynamic shared object loading
using `dlopen` and `dlsym`.

It provides a minimal, RAII-based interface for loading shared objects,
resolving symbols, and managing library lifetimes safely and predictably.

The design goal is simplicity, correctness, and low-level usability,
making it suitable for Linux, BSD, WSL, and Unix-like C++ projects.

---

## Features

- Header-only
- POSIX-only (`dlopen`, `dlsym`)
- RAII-based handle management
- Explicit symbol resolution
- Safe move semantics
- Optional global symbol loading
- No ABI impact
- Suitable for plugin systems and loaders

---

## Installation

Simply place the header in your include path:

```cpp
#include <stdso>
