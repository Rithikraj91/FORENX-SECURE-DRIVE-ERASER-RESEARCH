# Existing Tools Comparison

| Feature | nwipe | hdparm | shred | ForenX |
|---|---|---|---|---|
| Whole-drive focus | Yes | Low-level utility | No | Yes |
| File-level focus | No | No | Yes | Yes |
| Device-level operations | Yes | Yes | No | Planned |
| HDD | Yes | Yes | Indirect | Planned |
| SSD/NVMe awareness | Yes | Device-dependent | Limited | Planned |
| Verification | Yes | Limited/tool-dependent | Limited | Planned |
| Metadata handling | Not primary | No | No | Planned |
| Slack-space focus | Not primary | No | No | Planned |
| Audit trail | Limited | No | No | Planned |
| Tamper-evident logging | Not core | No | No | Planned |

## Lessons for ForenX

- Learn from established device detection and verification workflows.
- Use device-native sanitization where appropriate.
- Do not blindly copy historical overwrite schemes.
- Make storage-specific limitations visible.
- Combine safe UI, sanitization, validation and auditability.
