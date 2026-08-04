# Vespria — Assets

Public image assets for the Vespria world: NPC portraits, region map tiles, and
location art.

This repository exists to be *served*, not read. Files here are delivered over
jsDelivr and referenced from the world's `portraitUrl` / `imageUrl` fields:

```
https://cdn.jsdelivr.net/gh/PrincepsFerrous/Vespria-Assets@main/npcs/<name>.png
```

It contains images only. The world itself — quests, factions, lore, and all
hidden information — lives in a separate private repository.

## Layout

| Path | Contents | Frame |
|------|----------|-------|
| `npcs/` | Character portraits | 1000×1000 |
| `regions/` | Region map tiles | 1024×1024 |
| `locations/` | Location art | 750×1333 |

Images are published here by `.claude/skills/codex-image/scripts/upload-image.mjs`
in the world repository, which commits, pushes, and writes the resulting URL back
into the owning entry.
