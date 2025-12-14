# Squirrel_color_scheme

入力メソッドにちょっとした輝きを ✨ — macOS風の軽やかなスキン（日間 / 夜間）。フロステッドな半透明、柔らかな角、システム風のハイライト色を備えた配色集です。Squirrel互換の入力方式向けに調整済み。

**概要**
- **プロジェクト名**: `Squirrel_color_scheme` — Squirrel / 互換入力メソッド用の配色プリセット集。
- **含まれるファイル**: `squirrel.custom.yaml`（`macos_native_light` と `macos_native_dark` の2プリセットを含む）。
- **特徴**: フロステッド半透明（translucency）、柔らかい角丸、システムブルーに近いハイライト、読みやすい注釈やラベル。

**クイックプレビュー**
- 日間（`macos_native_light`）: 透き通る白背景＋軽い影で、さっぱりした見た目。✅
- 夜間（`macos_native_dark`）: 落ち着いたダークグレー＋適度な透明度で目に優しい。🌙
- 両テーマともハイライト色を統一して認識しやすくしています。

**色の形式について**
- 色は `0xBBGGRR` の16進形式で指定します（注意：通常の `0xRRGGBB` ではなく BGR の並びです）。
  - 例: `hilited_candidate_back_color: 0xFF7A00`（YAML内のコメントに RGB ↔ BGR の対応があります）。

**インストール（簡単）**
1. リポジトリの `squirrel.custom.yaml` を使用している入力メソッドの設定ディレクトリにコピーします（入力メソッドによってパスは異なります）：

```bash
cp squirrel.custom.yaml ~/Library/Rime/
# または
cp squirrel.custom.yaml ~/Library/Preferences/Squirrel/
```

2. 入力メソッドを再読み込みまたは再起動します（または deploy/reload コマンドを使用）。

ヒント: 既にカスタム設定がある場合は、該当するテーマセクションだけを既存の設定にマージしてから再読み込みしてください。

**設定例（ファイルから抜粋）**
- テーマ: `macos_native_light` / `macos_native_dark`
- ハイライト背景: `hilited_candidate_back_color: 0xFF7A00`
- 候補文字（昼）: `candidate_text_color: 0x222222`
- 注釈色: `comment_text_color: 0x999999`

**カスタマイズ方法**
- `squirrel.custom.yaml` の目的のテーマ（例: `macos_native_light`）を編集します：
  - フォント: `font_face`, `font_point`
  - 透明度: `alpha`, `translucency`
  - 角・影: `corner_radius`, `shadow_size`
  - 色: `back_color`, `hilited_candidate_back_color` など（`0xBBGGRR` を使用）

保存して再読み込みすれば、見た目を調整できます。

**貢献・フィードバック**
- 気に入ったら ⭐️ をお願いします。
- もっとテーマが欲しい（ハイコントラスト、色覚対応、季節限定色など）場合は Issue や PR を送ってください。
- PR にはプレビュー画像（png/jpg）を添付するとレビューが楽になります。

**ライセンス**
- ライセンス情報はリポジトリルートの `LICENSE` ファイルをご覧ください。