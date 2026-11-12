# OOP-Practical-4: RAII and Smart Pointers

## Purpose & Aim
- **Aim**: To learn how RAII ties resource lifetime to object lifetime and reduces manual memory-management errors.
- **Question**: Replace suitable raw new/delete usage with std::unique_ptr and std::shared_ptr. Compare behaviour and check for memory leaks.

---

## What to Do
- Create a small demo that allocates an object or array using std::unique_ptr.
- Create a second example where two parts of a program genuinely need shared ownership and use std::shared_ptr.
- Display or explain the ownership difference: unique_ptr has one owner; shared_ptr allows shared ownership.
- Avoid using shared_ptr when unique_ptr is sufficient. Do not manually delete smart-pointer-managed objects.
- Run the program through many iterations and compare its behaviour with a raw-pointer version if your instructor asks for a comparison.
- Use Valgrind or AddressSanitizer to check memory handling. Optionally record runtime or peak-memory observations using a system tool.
