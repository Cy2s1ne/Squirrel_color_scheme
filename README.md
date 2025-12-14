# Squirrel_color_scheme

[中文](README.md) · [English](README.en.md) · [日本語](README.ja.md)

给你的输入法换一套「会发光的」皮肤 ✨ — 轻盈的 macOS 风格（日间 / 夜间），磨砂、圆角、系统高亮色，一份小巧但有质感的配色集合。

**简介**
- **项目名**：`Squirrel_color_scheme` — 为 Squirrel / 兼容输入法准备的配色预设集合。
- **包含文件**：`squirrel.custom.yaml`（内含 `macos_native_light` 和 `macos_native_dark` 两套精心调校的预设）。
- **风格亮点**：磨砂半透明（translucency）、柔和圆角、系统蓝高亮、清晰的注解与序号样式。

**快速预览**
- 日间（`macos_native_light`）：通透白底 + 轻柔阴影，清爽且不抢眼。✅
- 夜间（`macos_native_dark`）：沉稳深灰 + 适度透明度，保护视力同时保留层次感。🌙
- 两套主题都使用一致的高亮色（近似 macOS 系统蓝），保证在不同背景下都有良好识别度。

**颜色格式说明**
- 配色项使用十六进制格式 `0xBBGGRR`（注意：这是 BGR 排列，不是常见的 `0xRRGGBB`）。
  - 例如：`hilited_candidate_back_color: 0xFF7A00`（配置中注释有 RGB ↔ BGR 的说明）。

**安装（超级简单）**
1. 把仓库根目录的 `squirrel.custom.yaml` 复制到你的输入法配置目录（不同输入法路径可能不同）：

```bash
cp squirrel.custom.yaml ~/Library/Rime/
# 或者
cp squirrel.custom.yaml ~/Library/Preferences/Squirrel/
```

2. 重新加载或重启输入法（或使用输入法提供的部署/重载命令）。

提示：如果你已有自定义配置，建议把文件中相应主题段落合并到现有配置再重载。

**快速示例（摘自配置）**
- 主题：`macos_native_light` / `macos_native_dark`
- 高亮背景：`hilited_candidate_back_color: 0xFF7A00`
- 候选文字（日间）：`candidate_text_color: 0x222222`
- 注解颜色：`comment_text_color: 0x999999`

**如何自定义（小白也能上手）**
- 打开 `squirrel.custom.yaml`，找到目标主题（例如 `macos_native_light`），修改：
  - 字体：`font_face`, `font_point`
  - 透明度：`alpha`, `translucency`
  - 圆角/阴影：`corner_radius`, `shadow_size`
  - 颜色：`back_color`, `hilited_candidate_back_color` 等（记得用 `0xBBGGRR`）

改好后保存，重载输入法看看效果；不满意就调参数，边改边看很方便。

**贡献与反馈**
- 喜欢这个配色？欢迎给个 ⭐️。
- 想要更多风格（高对比、色弱友好、节日限定色）或平台安装脚本？提 Issue 或发 PR 吧！
- 提交 PR 时请附上预览截图（png/jpg），好评审也好展示。

**许可**
- 本项目包含 `LICENSE` 文件，请查看仓库根目录的 `LICENSE` 了解授权信息。
