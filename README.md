# foldedhorizons-ae2

Applied Energistics 2 integration module for the **Folded Horizons** companion mod.

Will live at [`folded-horizons/folded-horizons-ae2`](https://github.com/folded-horizons/folded-horizons-ae2).

## What it ships

AE2Bridge (cross-dimensional ME grid access) and the ME backend for Trade Posts.

Depends on `foldedhorizons` (core) as a maven coordinate — see
[`folded-horizons/folded-horizons-core`](https://github.com/folded-horizons/folded-horizons-core)
for the core mod and its SPIs. Design docs:
[`folded-horizons/folded-horizons`](https://github.com/folded-horizons/folded-horizons)
→ `docs/companion-mod/`.

## Building

```sh
gradle build
```

Requires Java 21.
