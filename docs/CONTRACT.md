# Lore contract

Do not implement against folklore. Implement against this file.

## Identity

- Product: **Lore**
- Repo: `computerpets-lore`
- Category: Community
- Idea: Pet Lore Wiki
- Port / surface: `5173`

## Must

- Stay canon with 210 species. No illegal hybrids. No swapped voices.
- Treat the desktop overlay as the main quest. This organ is optional until wired.
- Fail soft: the overlay keeps walking if this service is down, unless this *is* the overlay.
- No PII in public artifacts (Steam id, wallet, home path, webcam frames).

## Data

SpeciesPage(id, habitat, taboo) · LineagePage(root, notable[]) · CanonTerm(name, kind)

## Surface

- GET /species/{id} — canon page
- GET /lineages/{id} — notable whelps
- POST /v1/lint — text vs canon names

## Neighbors

- computerpets-cortex
- computerpets-kennel
- computerpets-atelier
- computerpets-babel

## Failure doctrine

Missing art → silhouette, never a wrong photo. Lint fail in Cortex → block the line. Manual edits live in /canon and win over generation.

## Stack

TypeScript · VitePress / Astro · generated species pages from flagship data · canon lint
