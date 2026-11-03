---
"@biomejs/biome": patch
---

Fixed [#12908](https://github.com/biomejs/biome/issues/12908): `--write` no longer requests write access to files it doesn't change. Read-only files that need no changes no longer fail with a permission error, and unchanged files are no longer copied up on overlay filesystems. When a file changes on disk while Biome processes it, Biome now reports an error and leaves the file alone instead of overwriting it.
