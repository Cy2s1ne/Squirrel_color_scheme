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
1. `squirrel.custom.yaml` を設定ディレクトリにコピー（Squirrel は `~/Library/Rime/` のみ読み込みます）：

```bash
cp squirrel.custom.yaml ~/Library/Rime/
```

2. メニューバーの「鼠鬚管」→「再デプロイ」（または入力メソッドを再起動）。

> ⚠️ `*.custom.yaml` はパッチファイルで、**先頭に `patch:` が必要**です。無いと Rime はファイル全体を黙って無視し、「デプロイしたのに変わらない」状態になります。デプロイ後に `grep macos_native ~/Library/Rime/build/squirrel.yaml` で確認できます。

ヒント: 既にカスタム設定がある場合は `patch:` 以下の `style/...` と `preset_color_schemes/...` だけをマージ。

**有効化 / 切替**
`patch:` 以下に設定：
- `"style/color_scheme": macos_native_light`
- `"style/color_scheme_dark": macos_native_dark`

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
