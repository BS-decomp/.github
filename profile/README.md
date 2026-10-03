# BS-decomp

Unofficial, community-driven recovery of **Block Strike** Unity projects, version by version, from the original Android releases.

For each game version we take the original APK, export the Unity project, repair what the export and editor migration break — scenes, static-batch geometry, shaders, lightmaps, script references — and publish the result as a working Unity project, together with the recovery tooling and technical notes.

**This is not an official Block Strike project and not a game distribution.** The goal is study, preservation, and repair. Block Strike is developed by Rexet Studio; all rights to the game and its content belong to their respective owners.

## Repositories

| Version | Repository | Status |
| --- | --- | --- |
| 1.8.1 | [BS-decomp/1.8.1](https://github.com/BS-decomp/1.8.1) | 🕓 Planned — repository created, recovery not started |
| 3.7.0 | [BS-decomp/3.7.0](https://github.com/BS-decomp/3.7.0) | ✅ Published — recovered Unity project, recovery tools, technical docs |
| 4.1.0 | [BS-decomp/4.1.0](https://github.com/BS-decomp/4.1.0) | 🚧 In development — repository bootstrapped, APK confirmed (Unity 4.7.2f1, Mono, 58 scenes), export and repair in progress |
| 5.0.4 | — | 🕓 Planned |
| 6.5.1 | [BS-decomp/6.5.1](https://github.com/BS-decomp/6.5.1) | 🚧 In development — recovered project, tooling, and docs are being published incrementally |
| others | — | 💤 Under consideration, depending on available sources |

Repository names follow the game version (`<major>.<minor>.<patch>`).

## What a version repository contains

Most version repositories follow the same layout:

| Path | Contents |
| --- | --- |
| `client/` | Recovered Unity project: scenes, scripts, assets, and editor tooling |
| `original/` | Reference material from the original Android release (e.g. the APK) |
| `tools/` | Scripts and Unity editor tools reproducing parts of the recovery process |
| `docs/` | Technical notes: export status, scene names, geometry, shaders, lightmaps, compatibility |
| `AGENTS.md` | Working rules for agents and contributors, where present (in Russian) |

The recovered project in `client/` already contains the repairs known at publish time — you do not need to run any installer scripts just to open it. Open `client/` in the Unity version listed in that repository's README; the target editor and the Unity version of the original build both differ between game versions (for example, 3.7.0 targets **Unity 5.6.7f1**, while 6.5.1 targets **Unity 2021.3.45f2 LTS**).

## Limitations

These are reconstructions, so bugs, missing functionality, and differences from the original game are possible. Opening a scene in the editor does not guarantee that an Android build or online gameplay will work: some platform integrations and services depend on components outside the recovered Unity project.

## Contributing

Issues and fixes are welcome. When reporting a problem, please include:

- the game version and repository,
- the scene or feature involved,
- steps to reproduce,
- your Unity version,
- any relevant logs or screenshots.

## Rights

Block Strike and its original content belong to Rexet Studio and their respective rights holders. The presence of a LICENSE file in a repository does not by itself grant permission to redistribute the original game, APK, or third-party assets; please respect their applicable rights when using these repositories. Rights holders may contact organization members regarding any concerns.
