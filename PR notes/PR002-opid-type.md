# PR 2: Define OpId Type

## Goal

Implement the `OpId` type that uniquely identifies operations in the CRDT.

Every operation in our CRDT needs a unique identifier. This ID helps track which operation is which, especially when operations happen at the same time on different devices. Think of it like a unique stamp on each edit.

## What to Build

- An `OpId` struct with two numbers: `client_id` and `seq`
- The ability to create new `OpId` values
- The ability to compare `OpId` values (equal, greater than, less than)
- Helper methods to get the values from an `OpId`

## Reading List

### Rust Types & Structs

**The Rust Book - Chapter 5: Using Structs to Structure Related Data**
- https://doc.rust-lang.org/book/ch05-00-structs.html
- Learn how to define structs, add methods, and organize data

**The Rust Book - Chapter 3: Common Programming Concepts - Data Types**
- https://doc.rust-lang.org/book/ch03-02-data-types.html
- Understand primitive types like `u64`

### Traits (Derive Macros)

**The Rust Book - Appendix C: Derivable Traits**
- https://doc.rust-lang.org/book/appendix-03-derivable-traits.html
- Understand what traits like `Clone`, `Copy`, `Debug`, `Eq`, `Ord` do and when to derive them

### CRDT Background

**Shapiro et al. - A Comprehensive Study of Convergent and Commutative Replicated Data Types**
- https://hal.inria.fr/inria-00555588/document
- Read sections 1-3 to understand what CRDTs are and why operation identity matters
- Focus on understanding why each operation needs a unique ID

### Optional (for deeper understanding)

**Rust by Example - Traits**
- https://doc.rust-lang.org/rust-by-example/trait.html
- Learn more about traits to understand what's happening under the hood

