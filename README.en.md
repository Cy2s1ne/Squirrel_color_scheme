# Squirrel_color_scheme

Give your input method a little jelly glow ✨  
A lightweight macOS-style skin (Light / Dark) with frosted translucency, soft corners, and system-blue highlights.

**What is this**
- Theme presets for Squirrel / Rime on macOS.
- `squirrel.custom.yaml` includes `macos_native_light` and `macos_native_dark`.
- A shared highlight color keeps recognition crisp.

**Where it works**
- Squirrel / Rime on macOS (or compatible skins).

**30-second setup**
1. Copy `squirrel.custom.yaml` to your config directory (Squirrel only reads `~/Library/Rime/`):

```bash
cp squirrel.custom.yaml ~/Library/Rime/
```

2. Menu bar "Squirrel" → "Deploy" (or restart the input method).

> ⚠️ `*.custom.yaml` is a patch file: it **must start with `patch:`**. Without it Rime silently ignores the whole file — the patch deploys but nothing changes. Verify after deploying with `grep macos_native ~/Library/Rime/build/squirrel.yaml`.

Tip: if you already have custom configs, merge only the `style/...` and `preset_color_schemes/...` entries under `patch:`.

**Enable / switch themes**
Under `patch:`, set:
- `"style/color_scheme": macos_native_light`
- `"style/color_scheme_dark": macos_native_dark`

**Color format**
- Colors use hex `0xBBGGRR` (BGR order, not `0xRRGGBB`).
  - Example: `hilited_candidate_back_color: 0xFF7A00` (RGB 0,122,255 -> BGR FF7A00).

**Tweak knobs**
- Fonts: `font_face`, `font_point`
- Transparency: `alpha`, `translucency`
- Corners/shadow: `corner_radius`, `shadow_size`
- Colors: `back_color`, `hilited_candidate_back_color`, `candidate_text_color`, etc.

Save and reload to see changes.

**Contribute & Feedback**
- Like it? Drop a ⭐️.
- Want more flavors (high contrast, color-blind friendly, seasonal)? Open an Issue / PR.
- Please include preview screenshots (png/jpg) in PRs.

**License**
- See `LICENSE` in the repo root.
