# Custom Memory Allocation Library

## Overview
A custom memory management implementation in C++ using manual heap manipulation and tracking.

## Key Features
- Custom `malloc()` replacement
- Dynamic memory allocation tracking
- Block splitting and merging
- Buffer overrun protection
- Minimal external memory library dependencies

## Functions
- `malloc()`: Allocate memory blocks
- `free()`: Release memory blocks
- `calloc()`: Allocate and zero-initialize memory
- `malloc_called_count()`: Track allocation calls
- `used_blocks_count()`: Count active memory blocks

## Memory Management Techniques
- Manual heap segment expansion/contraction
- Metadata-based block tracking
- Adaptive block splitting
- Adjacent block merging

## Compilation
- Requires C++11 or later
- No external memory library dependencies

## Usage
```cpp
snp::Memory::malloc(size_t size);
snp::Memory::free(void* ptr);
```

## Safety Features
- Double-free prevention
- Buffer overrun detection
- Boundary checking

