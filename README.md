# Pehkui — Resize Any Mob

Scale is not a cosmetic layer in this mod. Shrink a mob and it stops reaching the lever it used
to pull; grow it and it starts bumping its head on the ceiling it used to walk under. Hitboxes,
step height, reach, fall damage, even the camera all follow the number you set, which is why a
tiny villager behaves like a tiny villager instead of a normal one wearing a small costume.

That single idea opens up a lot: pocket-sized pets that ride on a shoulder, a boss that genuinely
towers over the arena, a one-block-high crawlspace that only a shrunken player can get through.

## What this build is

An unofficial rebuild of **Virtuoel's** original work, kept running on current releases by
9Minecraft Studios. Not affiliated with the original author and not endorsed by them.

The porting work is mostly in the mixin layer. Each Minecraft release moves or renames the
methods this mod hooks into — entity dimensions, the camera transform, the attribute system —
so the hooks get re-pointed and re-tested rather than rewritten. The scaling maths underneath is
upstream's and is left alone on purpose: that is the part that makes the mod feel right, and it
is not ours to redesign.

## In this repository

- `build.gradle`, `gradle.properties`, `settings.gradle` — the build as it actually runs
- `src/` — a readable slice of the port: the mixin entry points that had to move
- `LICENSE` — upstream's terms, unchanged

The full tree is not mirrored here. If you want it for review, for a fork, or to build it
yourself, ask at **9minecraft.net@gmail.com** and it will be sent over.

## Building

```
./gradlew build
```

Artefacts land in `build/libs/`. You will need a JDK matching the Minecraft release you are
targeting — the wrapper handles the rest.

## Getting the built mod

If you would rather not build it, the finished jars are posted with install steps, the
dependency list, and the changelog for each release, here:
[9minecraft.net/pehkui-9minecraft-mod](https://www.9minecraft.net/pehkui-9minecraft-mod/)

## Credits

Original mod by **Virtuoel**. Licensed MIT; the upstream licence text ships inside every build.
Port and maintenance by 9Minecraft Studios.
