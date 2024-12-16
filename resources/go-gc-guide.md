# Go Garbage Collection Guide

The Go garbage collector (GC) plays a crucial role in managing memory. Mongosync performance can be improved by fine-tuning GC parameters.

## Key Parameter: GOGC
- `GOGC` defines the percentage of heap growth at which garbage collection is triggered.
- Example: `GOGC=100` means garbage collection starts when the heap grows by 100%.

### Adjusting GOGC
Set `GOGC` based on your server's CPU and memory availability:
```bash
export GOGC=50

For further details, refer to the official Go GC guide: https://tip.golang.org/doc/gc-guide.