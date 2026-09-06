# Drive Verification and Validation

A drive erasure workflow should not end with “Done”.

```text
Sanitization
    ↓
Verification / Validation
    ↓
Result
```

Possible outcomes:

- SUCCESS
- FAILED
- CANCELLED
- PARTIAL / UNKNOWN

The result should contain the target, method, timestamps, operation status, validation result and relevant errors.

Verification must be based on what the selected sanitization mechanism can actually establish. For SSD/NVMe, the software should not claim physical NAND verification that it cannot perform.
