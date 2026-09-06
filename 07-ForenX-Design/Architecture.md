# ForenX Architecture

## Conceptual Architecture

```text
                         USER
                           |
                           v
                    FORENX UI
              React + TypeScript
                     Tailwind
                           |
                           v
                         Tauri
                           |
                           v
                    Backend / API
                        FastAPI
                           |
                           v
                 ERASER ORCHESTRATOR
                           |
          +----------------+----------------+
          |                |                |
          v                v                v
      Discovery       Sanitization     Verification
                           Engine           Engine
          |                |                |
          +----------------+----------------+
                           |
                           v
                       Rust Core
                           |
                    C++ FFI where
                       required
                           |
                           v
              OS / Hardware Interfaces
                     /           \
                  SATA          NVMe
```

## Storage and Audit

```text
Audit Manager
     |
 +---+---+
 |       |
SQLite  RocksDB
 |       |
 +---+---+
     |
  SHA-256
 hash chain
```

This is a conceptual mapping based on the proposed architecture. Final technology choices should be confirmed during technical design.
