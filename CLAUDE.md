# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a cartographic/mapping project for Nyari Estate (Nairobi, Kenya). The workflow is:
- Manually trace satellite imagery using Inkscape to create vector estate maps
- Maintain version-controlled outputs for estate management purposes

## File Relationships

This project uses a layered file structure:

| Layer | Files | Purpose |
|---|---|---|
| Working source | `NyariMap2026.odg`, `NyariMap2026Lines.odg`, `NyariMap2026LinesWithImage.odg` | Editable Inkscape/LibreOffice Draw source files |
| Master export | `NyariEstateMaps.svg` | Full-detail vector export (13MB, ~7,170 lines) |
| Distribution | `NyariEstateMaps.pdf`, `NyariMap2026.pdf` | Print/share exports |
| Reference imagery | `*.png`, `*.jpg`, `NAIROBI BLOCK 94 Site plan.pdf` | Satellite and aerial imagery used as tracing references |
| Specialty | `Barrier.svg` | Standalone barrier element assets |

## Map Regions

The estate map is divided into named sections:
- **Nyari West** — Includes numbered plots (e.g., 85, 87)
- **Nyari Central**
- **Good News**
- **Upper Nyari**
- **Lower Lake Houses**

Each section has individual plot numbering. Commits are typically tagged with the region name and plot numbers changed (e.g., "numbers 85 and 87 added to Nyari West").

## Workflow

1. Edit the source `.odg` file in Inkscape or LibreOffice Draw
2. Export/save to `NyariEstateMaps.svg` (the master vector file)
3. Export to PDF as needed (`NyariEstateMaps.pdf` for full detail, `NyariMap2026.pdf` for smaller reference)
4. Commit all changed files together

## Git Repository

Remote: `git@github.com:drneal/Nyari-Map.git` (GitHub)

Commit messages follow the pattern: describe what was added/changed and in which region. Example: `"numbers 85 and 87 added to Nyari West"`.
