# scoop-bucket

[Scoop](https://scoop.sh) bucket for [meSingh](https://github.com/meSingh)'s tools.

```powershell
scoop bucket add mesingh https://github.com/meSingh/scoop-bucket
scoop install polinrider-cleaner
polinrider-check -Roots C:\work
```

| App | What it is |
|---|---|
| [`polinrider-cleaner`](bucket/polinrider-cleaner.json) | The Windows check from [polinrider-cleaner](https://github.com/meSingh/polinrider-cleaner): finds and quarantines PolinRider artifacts on one machine. Read-only unless you pass `-Apply`. |

Manifests install from the signed release tarballs and pin the release checksum. `checkver` and `autoupdate` track new releases via the published `SHA256SUMS`.
