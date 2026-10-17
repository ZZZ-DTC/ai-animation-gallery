# Model & Generation Notes

用于记录每个动画的生成上下文，方便复盘和横向比较。未知字段可以暂时填写 `待补充`。

## Works

| Work | File | Model | Version | Date | Human edits |
|---|---|---|---|---|---|
| Pelican on a Bicycle | `animations/pelican-on-bicycle.html` | 待补充 | 待补充 | 待补充 | 无 / 待补充 |
| Kitsune Express | `animations/kitsune-express-fox-on-bicycle.html` | 待补充 | 待补充 | 待补充 | 无 / 待补充 |

## Entry template

```yaml
id: work-000
name: "作品名称"
html: "animations/example.html"
preview: "assets/example.gif"
model: "模型名称"
model_version: "模型版本"
generated_at: "YYYY-MM-DD"
prompt: |
  在这里粘贴完整提示词。
human_edits:
  - "无"
format: "single-file HTML"
techniques:
  - "SVG"
  - "CSS animation"
notes: |
  视觉效果、运动节奏、代码结构和可复用性评价。
score:
  visual: 0
  motion: 0
  code: 0
  overall: 0
```

## Suggested evaluation dimensions

- **Visual**：构图、颜色、细节、可读性
- **Motion**：循环是否自然、节奏是否稳定、运动是否符合物理直觉
- **Code**：结构、可读性、依赖情况、可移植性
- **Overall**：作为可分享作品的综合完成度
