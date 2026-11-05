# scoop-bucket

[Scoop](https://scoop.sh) bucket for [meSingh](https://github.com/meSingh)'s tools.

```powershell
scoop bucket add mesingh https://github.com/meSingh/scoop-bucket
scoop install polinrider-scanner
polinrider
```

| App | What it is |
|---|---|
| [`polinrider-scanner`](bucket/polinrider-scanner.json) | The [polinrider-scanner](https://github.com/meSingh/polinrider-scanner) binary: checks this machine, local repositories and GitHub accounts and organizations for the PolinRider campaign. Read-only unless you pass `--apply`. |

Manifests install the prebuilt release binaries and pin the release checksum. `checkver` and `autoupdate` track new releases via the published `SHA256SUMS`.

`polinrider-scanner` was called `polinrider-cleaner` up to 2.3.0. The old
manifest is in [`deprecated/`](deprecated/polinrider-cleaner.json), where
`scoop status` reports it as deprecated, and it gets no updates. To move to the
new name:

```powershell
scoop uninstall polinrider-cleaner
scoop install polinrider-scanner
```
