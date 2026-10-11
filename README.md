# scoop-bucket

[Scoop](https://scoop.sh) bucket for [meSingh](https://github.com/meSingh)'s tools.

```powershell
scoop bucket add mesingh https://github.com/meSingh/scoop-bucket
scoop install polinrider-cleaner
polinrider
```

| App | What it is |
|---|---|
| [`polinrider-cleaner`](bucket/polinrider-cleaner.json) | The [polinrider-cleaner](https://github.com/meSingh/polinrider-cleaner) binary: checks this machine, local repositories and GitHub accounts and organizations for the PolinRider campaign. Read-only unless you pass `--apply`. |

Manifests install the prebuilt release binaries and pin the release checksum. `checkver` and `autoupdate` track new releases via the published `SHA256SUMS`.
