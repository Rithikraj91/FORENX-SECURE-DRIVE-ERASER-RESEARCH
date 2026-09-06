# Secure File & Metadata Eraser

## Purpose

Process selected files/folders and associated metadata, while accounting for filesystem and storage limitations.

## Workflow

```text
Select File/Folder
  ↓
Target Analysis
  ↓
Filesystem Detection
  ↓
Media Detection
  ↓
Content + Metadata Handling
  ↓
Appropriate Erasure
  ↓
Validation
  ↓
Audit Trail
  ↓
Final Result
```

## File Content

File content is the actual stored information.

## Metadata

Examples include:

- Filename
- Size
- Timestamps
- Permissions
- Ownership
- Filesystem-specific attributes

## Folder Handling

A folder operation should enumerate relevant files and subfolders rather than treating the directory entry as the only target.

## Important Limitation

On SSD/NVMe, host-level file operations cannot necessarily establish that every physical NAND location previously associated with the file has been sanitized.
