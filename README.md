# Lore

**Pet Lore Wiki** — Auto-generated wiki documenting rare pet lineages, species canon, and illegal hybrids.

Part of the [ComputerPets](https://github.com/RicheyWorks/computerpets) ecosystem. Index: [computerpets-ecosystem](https://github.com/RicheyWorks/computerpets-ecosystem).

> Status: **design scaffold**. This repository ships the contract, README, and layout so implementation can start without renaming the organ later.

## Why it exists

210 living kinds. Lore is the book so Cortex, Kennel, and Atelier do not invent a quiet line back into existence — or a panda-fish.

The flagship overlay already puts a living sticker on the real desktop (Rui first, 210 kinds). Lore does not replace that. It is one organ.

## Stack

TypeScript · VitePress / Astro · generated species pages from flagship data · canon lint

GroupId / namespace: `com.enterprisepet.lore`  
Default listen: `5173`

## Talks to

- computerpets-cortex
- computerpets-kennel
- computerpets-atelier
- computerpets-babel

## Contract

### Data

`SpeciesPage(id, habitat, taboo) · LineagePage(root, notable[]) · CanonTerm(name, kind)`

### Surface

- GET /species/{id} — canon page
- GET /lineages/{id} — notable whelps
- POST /v1/lint — text vs canon names

### Failure doctrine

Missing art → silhouette, never a wrong photo. Lint fail in Cortex → block the line. Manual edits live in /canon and win over generation.

## Layout

```
computerpets-lore/
  README.md           this file
  LICENSE             MIT
  docs/CONTRACT.md    the same contract, frozen for implementers
  src/                implementation lands here
```

## Run (Windows)

PowerShell, from this folder, after the flagship helpers (Git, Node LTS 22+, JDK 21 as needed):

```powershell
npm install; npm run docs:dev
```

You do not need this service to meet Rui. The [flagship start-here](https://github.com/RicheyWorks/computerpets/blob/main/docs/START-HERE.md) is still the first pet.

## Ecosystem

| Organ | Repo |
| --- | --- |
| Flagship desktop + Spring | [RicheyWorks/computerpets](https://github.com/RicheyWorks/computerpets) |
| This organ | [RicheyWorks/computerpets-lore](https://github.com/RicheyWorks/computerpets-lore) |
| Full map | [RicheyWorks/computerpets-ecosystem](https://github.com/RicheyWorks/computerpets-ecosystem) |

## License

MIT. See [LICENSE](LICENSE).

---

*Two hundred ten living kinds. Keep them so a line does not go quiet.*
