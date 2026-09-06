# Audit and Tamper-Evident Logging

## Example Record

```text
Operation ID: FX-2026-00001
Timestamp: 2026-09-06 10:15:32
Target: <device/file identifier>
Media Type: SATA SSD
Method: <selected method>
Start: <timestamp>
End: <timestamp>
Result: SUCCESS
Validation: PASSED
Errors: NONE
```

## Hash Chaining

```text
Record 1 → Hash 1
Record 2 + Hash 1 → Hash 2
Record 3 + Hash 2 → Hash 3
```

Changing an earlier record changes its hash and can cause the chain to fail integrity checking.

Use the term **tamper-evident** rather than claiming absolute tamper-proof storage.
