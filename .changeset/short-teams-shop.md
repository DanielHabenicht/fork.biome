---
"@biomejs/biome": patch
---

Fixed [#12908](https://github.com/biomejs/biome/issues/12908): `--write` no longer requests write access to files it doesn't change. Read-only files that need no changes are no longer reported with "Permission denied", and unchanged files are no longer copied up on overlay filesystems.
