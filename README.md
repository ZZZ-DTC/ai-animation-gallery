# AI Animation Gallery

一个用于保存、查看和对比不同 AI 模型生成的 HTML / SVG 动画的静态画廊。

## 在线访问

启用 GitHub Pages 后，访问：

```text
https://<你的用户名>.github.io/ai-animation-gallery/
```

首页会同时提供：

- HTML 实时动画预览
- GIF 快照预览
- 原始 HTML 文件链接
- GIF 下载链接
- 模型与生成上下文记录入口

## 目录结构

```text
ai-animation-gallery/
├── index.html                         # GitHub Pages 首页
├── animations/                        # 可运行的原始 HTML 动画
│   ├── pelican-on-bicycle.html
│   └── kitsune-express-fox-on-bicycle.html
├── assets/                            # GIF 快照
│   ├── pelican-on-bicycle.gif
│   └── kitsune-express-fox-on-bicycle.gif
└── metadata/
    └── models.md                      # 模型、提示词和评价记录模板
```

## GitHub Pages 部署

1. 创建 GitHub 仓库，推荐名称：`ai-animation-gallery`
2. 将本目录中的文件上传到仓库根目录
3. 打开 **Settings → Pages**
4. 选择 **Deploy from a branch**
5. 选择 `main` 分支和 `/ (root)` 目录
6. 等待部署完成后访问 GitHub Pages 地址

也可以使用 Git：

```bash
git init
git add .
git commit -m "Add AI animation gallery"
git branch -M main
git remote add origin https://github.com/<你的用户名>/ai-animation-gallery.git
git push -u origin main
```

## 记录新作品

建议每个新作品至少保存：

- 一个可运行的 HTML 文件
- 一个统一命名的预览图或 GIF
- 使用的 AI 模型和版本
- 生成日期
- 完整提示词
- 人工修改内容
- 对动画质量、视觉效果和代码质量的评价

具体字段见 [`metadata/models.md`](metadata/models.md)。

## 说明

当前两个 HTML 均为单文件动画，图形资源内嵌在 SVG 中，不依赖外部图片或 JavaScript 资源，适合直接通过 GitHub Pages 发布。
