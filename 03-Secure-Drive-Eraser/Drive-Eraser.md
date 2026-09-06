# Secure Drive Eraser

## Purpose

Sanitize an entire storage device while providing strong safety controls, validation and auditability.

## Workflow

```text
Select Drive
  ↓
Device Discovery
  ↓
Device Identification
  ↓
Capability Detection
  ↓
Media Classification
  ↓
Method Selection
  ↓
Safety Confirmation
  ↓
Sanitization
  ↓
Verification / Validation
  ↓
Audit Trail
  ↓
Final Report
```

## Device Information

ForenX should identify, where available:

- Model
- Manufacturer
- Serial number
- Capacity
- Interface
- HDD/SSD/NVMe classification
- Partitions
- Mounted status
- System/boot-drive status
- Device capabilities

## Method Selection

“Multiple Erasure Algorithms” should be interpreted as multiple appropriate sanitization strategies, not simply many overwrite passes.

Examples:

- HDD: appropriate overwrite and/or supported device-level method.
- SATA SSD: supported ATA/device-level sanitization where appropriate.
- NVMe: supported NVMe sanitization mechanism where appropriate.
- Encrypted media: cryptographic erase where prerequisites are satisfied.

## Safety

The UI should clearly identify the exact target and warn about destructive consequences. System/boot drives require special protection.

## Verification

The system must distinguish successful, failed, cancelled and uncertain/partial outcomes. It must never report success when validation fails.
