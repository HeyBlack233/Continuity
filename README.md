# Disclaimer

This Repository is not affiliated with the original Continuity in any way.

Please report any issues to this Repository only.

## Continuity

The Continuity Fabric mod was ported to 1.16 by me. All credits go to the creator Pepper_Bell.

Continuity is a Fabric mod built around modern APIs to allow for the most efficient connected textures experience possible. It is designed to provide full Optifine parity for all resource packs that use the Optifine/MCPatcher CTM format.

Continuity depends on the Fabric API and is client-side only. With the mod come two built-in resource packs - one provides default connected textures, similar to Optifine, and the other provides a fix for glass pane culling.

## Development

This fork targets Minecraft 1.16.5 with a Java 26-only toolchain. The Gradle wrapper pins Gradle 9.8.2 and provisions Temurin 26 automatically, so a system Java installation is not required.

```sh
./gradlew build
./gradlew runClient
```

The first build downloads Gradle, Loom, Minecraft, mappings, Fabric API, and assets; later builds can use the Gradle cache.

## CTM

Nowadays, there are two main CTM (Connected Texture Mapping) formats:

- Optifine/MCPatcher format
- Chisel/ConnectedTexturesMod format

Continuity only supports the Optifine/MCPatcher format. If support for the Chisel format is required, consider using the [ConnectedTexturesMod for Fabric](https://www.curseforge.com/minecraft/mc-mods/ctm-fabric) instead. Note that using Continuity and CTMF at the same time is an unsupported configuration, at least for the time being.

## Forge Version

I do not see myself working on a Forge version of Continuity for two main reasons:

- Optifine. Optifine has native support for Forge, so a Forge version of Continuity would not be very useful in the first place.
- Forge's model API. It is vastly different from Fabric's model API (FRAPI), which is utilized by the Fabric version, and switching to it would not only require an incredible amount of effort, but also result in the mod being extremely inefficient.

### Links

[CurseForge Page](https://www.curseforge.com/minecraft/mc-mods/continuity)

[Modrinth Page](https://modrinth.com/mod/continuity)

[Discord](https://discord.gg/7rnTYXu)

[GitHub](https://github.com/PepperCode1/Continuity)
