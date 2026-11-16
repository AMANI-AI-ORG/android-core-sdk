## amani-kyc 3.24.0

### What's Changed

- feature: **Document capture loader colour** — `DocBuilder` takes `loaderColor` (colour resource) and `loaderColorHex` (`#RRGGBB` / `#AARRGGBB`, wins when valid) for the loader shown while a capture is processed. The previous `DocBuilder` constructor still works.
- improvement: **Full-resolution document capture** — document pages are captured at full camera resolution.
- improvement: **Document page cache** — captured pages are cleared automatically after a successful upload; a failed upload keeps them so the upload can be retried.
- improvement: **R8 full mode** — host apps can build with R8 full mode using only the rules bundled in the AAR.
- fix: **Manual crop state** — a manually cropped page no longer affects the `cropped` value of a later document in the same session.

### Checksums (SHA-256)

| File | SHA-256 |
|---|---|
| `AmaniAi-3.24.0-sources.jar` | `fe5bd3550128e48a5bbef16a45d7f9a0ab550a40f2c46d37906bae6ade83d5d0` |
| `AmaniAi-3.24.0.aar` | `5d5e42c4e38464013c77e65b9cd1735d746f76e40867eb5e8b6923d4ec1655ee` |
| `AmaniAi-3.24.0.pom` | `e5eaec0e54eb4f69166b2dc0c68ff4061b1358e5b85c3cd5980e30e1df1d4fcf` |

Verify a downloaded file:

```bash
shasum -a 256 AmaniAi-3.24.0.aar
```

or, with `SHA256SUMS` from this release in the same folder (checks the files you have):

```bash
shasum -a 256 -c SHA256SUMS --ignore-missing
```
