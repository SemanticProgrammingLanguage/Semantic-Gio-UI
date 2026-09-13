# Semantic module integrity

This directory is the Semantic translation target for Gio `v0.10.2`.

The original source remains in the sibling directory `gio-v0.10.2`. The
translation is not treated as complete: every source that could not be
exported is listed in `SEMANTIC-MODULE.json`.

Before embedding or importing this module, verify the package files with
`SHA256SUMS.txt` and validate every `.se` file with:

```powershell
Get-ChildItem -Recurse -Filter *.se | ForEach-Object {
    & "..\Semantic Programming Language.exe" semantic-validate $_.FullName
}
```

The Gio license is preserved verbatim in `LICENSE`. Gio is distributed under
the Unlicense or the MIT License.

