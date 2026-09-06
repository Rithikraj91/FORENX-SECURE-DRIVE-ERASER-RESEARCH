# Storage Fundamentals

## HDD

HDDs use magnetic platters and read/write heads. Host-side overwriting can be a viable sanitization technique in appropriate scenarios.

## SSD/NVMe

SSDs use NAND flash and controllers containing mechanisms such as:

- Flash Translation Layer (FTL)
- Wear leveling
- Garbage collection
- ECC
- Bad-block management
- Remapping

The host sees logical addresses, while the controller manages physical NAND.

## Deletion

A simplified deletion model:

```text
Before:  [PHOTO][SECRET][VIDEO][REPORT]
Delete:  [PHOTO][FREE][VIDEO][REPORT]
```

The filesystem can regard the previous location as free even though remnants may remain.

## Free vs Slack Space

- **Free space:** outside currently allocated file space.
- **Slack space:** unused portion inside allocated space associated with an allocation unit.

## HDD vs SSD

HDD and SSD/NVMe should not be treated identically because SSD controllers can relocate data internally.
