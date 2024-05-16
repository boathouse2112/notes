# Garbage Collectors

- Some definitions include ref-count
- "Tracing Garbage Collection" -- what Java, Go do

# Rooting
- Objects "directly" on the stack are roots
  - `directly` -- without going through other GC'd objects
- Do you need multiple roots? Can't you put everything but a single ROOT on the heap?

# Tracing
