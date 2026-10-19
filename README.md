# foldedhorizons-ae2

Applied Energistics 2 integration module for the **Folded Horizons** companion mod.

## What it ships

AE2Bridge (cross-dimensional ME grid access) and the ME backend for Trade Posts.

Depends on `foldedhorizons` (core) as a maven coordinate — see
[`folded-horizons/folded-horizons-core`](https://github.com/folded-horizons/folded-horizons-core)
for the core mod and its SPIs. Design docs:
[`folded-horizons/folded-horizons`](https://github.com/folded-horizons/folded-horizons)
→ `docs/companion-mod/`.

## Building

The core mod is a sibling repository, consumed as the maven artifact
`dev.foldedhorizons:foldedhorizons:<version>`. For local development,
publish it once:

```sh
# in a checkout of folded-horizons-core
gradle :core:publishToMavenLocal
```

Then build this module:

```sh
gradle build
```

Requires Java 21. CI does the same thing automatically: it checks out
the core repo, publishes it to mavenLocal, and builds this module.

## Dev container

`.devcontainer/` provides Java 21 + Gradle; open the repo in a
dev container and `gradle build` works without host setup.
