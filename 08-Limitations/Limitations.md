# Limitations

## SSD/NVMe Physical Visibility

The host may not know every physical NAND location previously used by a file.

## Backups and Copies

Local sanitization does not remove copies held in backups, snapshots, mirrors or cloud services.

## Device Firmware

Device-level commands depend on device implementation and capabilities.

## Power or Communication Failure

An interrupted operation may leave the final state uncertain and must be reported accordingly.

## Unsupported Hardware

Some devices may not provide the sanitization mechanism required for a desired assurance level.

## Assurance

ForenX should communicate the achieved assurance and limitations rather than making absolute claims that cannot be technically verified.
