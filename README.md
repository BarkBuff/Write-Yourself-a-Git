### Write Yourself a Git

A from-scratch, technical reconstruction of Git’s internal mechanisms — designed to reveal how version control systems manage data, history, and integrity at the byte level.

This project re-implements the **core primitives** of Git — **object storage, hashing, commit graphs, trees, and references** — in **Python**, with a focus on transparency and minimalism. It walks through how Git transforms files into **content-addressed objects**, builds **commit DAGs**, and maintains a consistent state across local and distributed repositories.

Each module mirrors a real Git subsystem:

* **Object Layer:** Implements SHA-1 hashing, blob and tree serialization, and compression.
* **Repository Layer:** Handles .git directory structure, refs, HEAD pointers, and branch logic.
* **Commit Engine:** Constructs commit objects, parents, and timestamps for reproducible history.
* **Storage & Retrieval:** Reads and writes Git objects using zlib compression and filesystem I/O.
* **CLI Interface:** Minimal command parser replicating `git init`, `git add`, `git commit`, and `git log`.

Beyond functionality, the project emphasizes **systems-level understanding** — how design decisions in Git balance **performance, data safety, and distributed coordination**.

Built not to replace Git, but to **understand every abstraction it hides** — from raw bytes to commit history, from disk to distributed truth.
