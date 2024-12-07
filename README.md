# Unsafe Rust: Modifying Vector via Raw Pointer after Modification

This repository demonstrates a common error in Rust involving unsafe code and vectors.  The `bug.rs` file shows code that attempts to modify a vector through a raw pointer after the vector has been modified.  This leads to undefined behavior.

The solution, found in `bugSolution.rs`, addresses the issue by avoiding direct manipulation of the vector's raw pointer and instead utilizing safe Rust methods for vector modification.