# Nazar Subtitles — base presets

The animation presets that **Nazar Subtitles** installs into DaVinci Resolve, and the fonts they use.

In Resolve: open a Nazar Title → **GENERATE** → **Base presets → Update from GitHub…**. Nazar downloads the
files listed in `manifest.json`, checks every one against its sha256, installs the fonts for the current user
and imports the presets into the Media Pool bin **Word Subtitle Presets / Nazar Base**. An older Nazar Base is
kept in the root bin *Nazar Base (previous versions)*; your own presets are never touched.

Restart DaVinci Resolve after an update so it picks up newly installed fonts.

## What is here

| File | What it is |
| --- | --- |
| `manifest.json` | version, file list, sizes and sha256 checksums, preset names, font licences |
| `base_presets.drb` | the presets, as a DaVinci Resolve bin export |
| `fonts/` | the fonts the presets use, with their licence texts |

Current set **2026.09.16.1**: `BASIC_Opacity`, `NZR_KARAOKE_BLACK`, `VIOLET_EMPH`.

Fonts: **Fira Sans Extra Condensed** and **Pacifico**, both under the
[SIL Open Font License 1.1](https://openfontlicense.org) (`fonts/*-OFL.txt`).

## Publishing a new set

In Resolve: **Base presets → Save my presets as base set…**, put the fonts in `fonts/` of the chosen folder,
then upload `manifest.json`, `base_presets.drb` and `fonts/` here. The version in `manifest.json` decides what
is newer, so raise it every time.
