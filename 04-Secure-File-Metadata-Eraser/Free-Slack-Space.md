# Free Space and Slack Space

## Free Space

Space that the filesystem currently considers available.

```text
[A][SECRET][B][C]
        ↓ delete
[A][FREE][B][C]
```

Free does not necessarily mean physically empty.

## Slack Space

Unused space within an allocated storage unit associated with a file.

```text
+------------------------------+
| File Data | Slack Space      |
+------------------------------+
```

Slack can contain remnants depending on filesystem and storage behavior.

## SSD Limitation

Logical free/slack-space cleaning does not automatically establish physical NAND sanitization because SSD controllers manage physical placement.

ForenX should report the assurance actually established.
