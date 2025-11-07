### Write Yourself a Git

A from-scratch exploration of how Git actually works under the hood.

This project rebuilds the essential internals of a version control system - **object storage, hashing, commit graphs, trees, and references**. All written in **py** to expose what really happens when code meets storage.
It’s a hands-on study in **systems programming**, **file system design**, and **data integrity**, focusing on performance, structure, and reproducibility.

The goal isn’t to recreate Git feature-for-feature, but to **deconstruct its architecture**; understanding how content-addressable storage, delta compression, and metadata tracking interact to make distributed version control possible.
Built to trace the invisible path between “git add” and your disk — from bytes to history.
