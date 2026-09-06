# Method Selection

## Principle

The sanitization method should be selected from:

1. Media type
2. Device capabilities
3. Required assurance
4. Applicable standards
5. Operational constraints

## Conceptual Decision Tree

```text
Drive
 ↓
Identify Media
 ├── HDD
 │    └── Evaluate suitable device-level/overwrite strategy
 ├── SATA SSD
 │    └── Evaluate supported ATA/device sanitization
 └── NVMe
      └── Evaluate supported NVMe sanitization
```

## Gutmann

Gutmann's 1996 35-pass scheme is historically important but was designed around historical magnetic recording technologies. It should not be treated as a universal modern requirement.

## Cryptographic Erase

Cryptographic erase sanitizes relevant encryption keys so that recovery of encrypted target data becomes infeasible when the required encryption/key-management conditions are satisfied.
