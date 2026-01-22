# Squirrel_color_scheme

入力メソッドにちょっとした「ゼリー感の輝き」✨  
軽やかな macOS 風スキン（日間 / 夜間）。フロステッド半透明、丸み、システムブルーのハイライト。

**これは何**
- macOS の Squirrel / Rime 用テーマ。
- `squirrel.custom.yaml` に `macos_native_light` と `macos_native_dark` を収録。
- ハイライト色を統一して読みやすく。

**対応環境**
- macOS の Squirrel / Rime（外観設定互換の入力メソッド）。

**30秒セットアップ**
1. `squirrel.custom.yaml` を設定ディレクトリにコピー：

```bash
cp squirrel.custom.yaml ~/Library/Rime/
# または
cp squirrel.custom.yaml ~/Library/Preferences/Squirrel/
```

2. 再読み込み / 再起動。

ヒント: 既にカスタム設定がある場合は `style` と `preset_color_schemes` だけをマージ。

**有効化 / 切替**
`style` に設定：
- `color_scheme: macos_native_light`
- `color_scheme_dark: macos_native_dark`

**色の形式**
- 色は `0xBBGGRR`（BGR 順、`0xRRGGBB` ではありません）。
  - 例: `hilited_candidate_back_color: 0xFF7A00`（RGB 0,122,255 -> BGR FF7A00）。

**調整ポイント**
- フォント: `font_face`, `font_point`
- 透明度: `alpha`, `translucency`
- 角/影: `corner_radius`, `shadow_size`
- 色: `back_color`, `hilited_candidate_back_color`, `candidate_text_color` など

保存して再読み込みすれば反映されます。

**貢献・フィードバック**
- 気に入ったら ⭐️ をどうぞ。
- もっと違う味（高コントラスト、色覚対応、季節限定色）が欲しいなら Issue / PR へ。
- PR にはプレビュー画像（png/jpg）を添付してください。

**ライセンス**
- ルートの `LICENSE` を参照してください。
