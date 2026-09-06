# FORENX — Secure Drive Eraser & Secure File/Metadata Eraser

Research and technical design documentation for the two ForenX Layer 3 erasure modules.

## Scope

This repository covers only:

1. **Secure Drive Eraser**
2. **Secure File & Metadata Eraser**

The research focuses on storage fundamentals, sanitization methods, HDD vs SSD/NVMe limitations, NIST SP 800-88 Rev. 2, existing tools, architecture, verification, safety, and audit logging.

## Repository Structure

- `01-Introduction/` — project scope and objectives
- `02-Storage-Fundamentals/` — HDD, SSD, deletion and storage concepts
- `03-Secure-Drive-Eraser/` — drive sanitization research
- `04-Secure-File-Metadata-Eraser/` — file, metadata, free/slack-space research
- `05-NIST-SP-800-88/` — NIST guidance
- `06-Existing-Tools/` — nwipe, hdparm and shred research
- `07-ForenX-Design/` — proposed architecture and workflow
- `08-Limitations/` — technical and assurance limitations
- `09-References/` — primary references

## Important terminology

**Deleted** does not necessarily mean **sanitized**.

ForenX should select methods according to storage technology and device capabilities rather than assuming that more overwrite passes always provide better security.

## NIST wording

ForenX should be described as **designed/aligned with NIST SP 800-88 Rev. 2 and applicable standards**, not as “NIST certified” unless a formal certification exists.
