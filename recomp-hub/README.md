# Recomp Hub catalog

`ports.json` is downloaded by Sessionist for macOS (Direct edition) when the
Recomp Hub checks for updates. It lets ports be added or fixed without a new
Sessionist release.

- A JSON array of port entries, the same shape as Sessionist's built-in catalog.
- An entry with the same `id` as a built-in port replaces it; new ids are added.
- A user's own local `ports.json` still overrides this file.
- Entries a given Sessionist version cannot read are skipped, not fatal.

Entries can carry build commands that run on users' Macs, so treat changes
here like code: only merge what you have reviewed.
