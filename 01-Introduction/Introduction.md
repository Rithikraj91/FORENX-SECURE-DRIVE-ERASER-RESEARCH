# Introduction

## Background

Normal file deletion generally removes or changes filesystem references and marks storage as available for reuse. It does not necessarily make the underlying data inaccessible.

Secure sanitization is therefore required when data must be rendered infeasible to recover for a given level of effort.

## ForenX Scope

This research covers two Layer 3 modules:

- Secure Drive Eraser
- Secure File & Metadata Eraser

## Objectives

- Understand HDD, SATA SSD and NVMe storage behavior.
- Study appropriate sanitization strategies.
- Understand file, metadata, free-space and slack-space implications.
- Study NIST SP 800-88 Rev. 2.
- Analyze existing erasure tools.
- Design a safe, verifiable and auditable ForenX workflow.
- Document limitations honestly.

## Core Principle

> Deleted ≠ Sanitized.

A successful ForenX operation should report what was actually performed and what level of assurance was established.
