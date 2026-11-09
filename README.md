# Squirrel_color_scheme

[中文](README.md) · [English](README.en.md) · [日本語](README.ja.md)

给你的输入法加一层「果冻光」✨  
轻盈的 macOS 风格（日间 / 夜间），磨砂半透明、圆角、系统蓝高亮。

**这是什么**
- macOS 上 Squirrel / Rime 的外观主题。
- `squirrel.custom.yaml` 内含 `macos_native_light` 与 `macos_native_dark` 两套方案。
- 统一高亮色，读起来更清晰。

**适用环境**
- macOS 下的 Squirrel / Rime（或兼容外观配置的输入法）。

**30 秒上手**
1. 复制 `squirrel.custom.yaml` 到配置目录（Squirrel 只读 `~/Library/Rime/`）：

```bash
cp squirrel.custom.yaml ~/Library/Rime/
```

2. 菜单栏「鼠须管」→「重新部署」（或重启输入法）。

> ⚠️ `*.custom.yaml` 是补丁文件，**最外层必须有 `patch:`**。缺少 `patch:` 时 Rime 会静默忽略整个文件，表现就是「部署了但皮肤没变」。部署后可自检：
> `grep macos_native ~/Library/Rime/build/squirrel.yaml` —— 有输出才算生效。

提示：如果你已有自定义配置，建议只合并 `patch:` 下的 `style/...` 与 `preset_color_schemes/...` 两段。

**启用 / 切换主题**
在 `patch:` 中设置：
- `"style/color_scheme": macos_native_light`
- `"style/color_scheme_dark": macos_native_dark`

**配色格式**
- 颜色使用十六进制 `0xBBGGRR`（BGR 顺序，不是常见的 `0xRRGGBB`）。
  - 例：`hilited_candidate_back_color: 0xFF7A00`（RGB 0,122,255 对应 BGR FF7A00）。

**可调旋钮**
- 字体：`font_face`, `font_point`
- 透明度：`alpha`, `translucency`
- 圆角/阴影：`corner_radius`, `shadow_size`
- 颜色：`back_color`, `hilited_candidate_back_color`, `candidate_text_color` 等

改好后保存并重载即可生效。

**贡献与反馈**
- 喜欢就点个 ⭐️，我会开心很久。
- 想要更多风格（高对比、色弱友好、节日限定色）欢迎提 Issue / PR。
- 提交 PR 时请附预览截图（png/jpg），方便展示与评审。

**许可**
- 许可信息见仓库根目录的 `LICENSE`。
