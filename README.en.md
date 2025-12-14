# Squirrel_color_scheme

Give your input method a little glow ✨ — a lightweight macOS-style skin (Light / Dark) with frosted translucency, soft corners, and system-like highlight colors. This is a compact but tasteful color scheme collection for Squirrel-compatible input methods.

**Overview**
- **Project**: `Squirrel_color_scheme` — a set of color presets for Squirrel (or compatible) input method skins.
- **Files included**: `squirrel.custom.yaml` (contains `macos_native_light` and `macos_native_dark` presets).
- **Highlights**: frosted translucency, soft corner radius, system-blue highlights, clear annotations and labels.

**Quick Preview**
- Light (`macos_native_light`): translucent white background + gentle shadow — fresh and unobtrusive. ✅
- Dark (`macos_native_dark`): deep grey + balanced translucency — comfortable at night. 🌙
- Both themes use a consistent highlight color (close to macOS system blue) for clear recognition.

**Color format**
- Colors use the hex format `0xBBGGRR` (note: this is BGR order, not the common `0xRRGGBB`).
  - Example: `hilited_candidate_back_color: 0xFF7A00` (see comments in the YAML for RGB ↔ BGR mapping).

**Installation (quick)**
1. Copy `squirrel.custom.yaml` to your input method config directory (paths vary by input method):

```bash
cp squirrel.custom.yaml ~/Library/Rime/
# or
cp squirrel.custom.yaml ~/Library/Preferences/Squirrel/
```

2. Reload or restart your input method (or use its deploy/reload command).

Tip: If you already have custom configs, merge the relevant theme sections into your existing file before reloading.

**Quick examples (from the file)**
- Theme: `macos_native_light` / `macos_native_dark`
- Highlight background: `hilited_candidate_back_color: 0xFF7A00`
- Candidate text (light): `candidate_text_color: 0x222222`
- Comment color: `comment_text_color: 0x999999`

**Customization (easy)**
- Open `squirrel.custom.yaml` and edit the theme section (e.g., `macos_native_light`):
  - Fonts: `font_face`, `font_point`
  - Transparency: `alpha`, `translucency`
  - Corners/shadow: `corner_radius`, `shadow_size`
  - Colors: `back_color`, `hilited_candidate_back_color`, etc. (use `0xBBGGRR`)

Save and reload — tweak until it looks right.

**Contribute & Feedback**
- Like this scheme? Give a ⭐️.
- Want more themes (high-contrast, colorblind-friendly, seasonal)? Open an Issue or send a PR.
- Please include preview screenshots (png/jpg) in PRs for easier review.

**License**
- See the `LICENSE` file in the repository root for license details.