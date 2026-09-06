# Functional and Safety Requirements

## Secure Drive Eraser

### Functional

- Discover storage devices.
- Identify device characteristics.
- Detect capabilities.
- Classify HDD/SATA SSD/NVMe.
- Select appropriate sanitization strategy.
- Execute supported operation.
- Validate result.
- Generate audit record.
- Generate final report.

### Safety

- Show exact target details.
- Detect system/boot drive.
- Detect mounted/in-use status.
- Require explicit confirmation.
- Require appropriate privileges.
- Prevent target mismatch.
- Handle cancellation and interruption.
- Never report false success.

## Secure File & Metadata Eraser

- Select file/folder.
- Identify filesystem.
- Identify underlying media type where possible.
- Handle content and metadata.
- Address relevant free/slack-space operations where appropriate.
- Validate.
- Record audit trail.
- Report limitations.
