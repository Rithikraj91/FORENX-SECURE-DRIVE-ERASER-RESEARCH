# Testing Plan

## Stage 1 — Safe Software Tests

Use:

- Mock device information
- Test files
- Virtual disks/images
- Simulated errors

Test:

- Device discovery
- Method selection
- UI warnings
- Validation logic
- Audit logging

## Stage 2 — Dedicated Hardware

Use disposable/test:

- HDD
- SATA SSD
- NVMe

No valuable data should be present.

Test:

- Successful operations
- Unsupported methods
- Device errors
- Interruption
- Verification failure
- Audit integrity

## Stage 3 — Integration

Integrate UI, backend, core and hardware interfaces only after isolated components behave correctly.
