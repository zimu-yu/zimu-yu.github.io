# Zimu Yu · 个人学术主页

采用 [AcademicPages](https://academicpages.github.io/) 官方学术主页结构：固定顶部导航、左侧个人资料、右侧正文，以及响应式的移动端个人链接菜单。网站继续使用 Jekyll 和 Markdown，并保留原有研究与论文信息。

## 以后只需改这些文件

| 想修改的内容 | 文件 |
| --- | --- |
| 名字、个人简介、所在地、邮箱、学术链接 | `_config.yml` 中的 `author` |
| 首页介绍、研究兴趣、动态 | `index.md` |
| 论文列表 | `_pages/publications.md` |
| 项目与研究 | `_pages/research.md` |
| 简历页面 | `_pages/cv.html`（只嵌入 PDF） |
| 书籍、工具、学习资源 | `_pages/resources.md` |
| 顶部栏目名称和顺序 | `_data/navigation.yml` |

在 GitHub 打开相应文件 → 点击铅笔编辑 → 保存提交。GitHub Pages 构建完成后网站更新。保留每个 Markdown 文件顶部两条 `---` 之间的配置。

## 换头像

上传照片到 `assets/images/avatar.jpg`，然后在 `_config.yml` 的 `author:` 下增加（注意两个空格缩进）：

```yaml
  avatar: "/assets/images/avatar.jpg"
```

没有设置头像时显示 ZY 字母头像。不会使用他人的照片。

## 添加一篇论文

复制到 `_pages/publications.md` 对应年份下面，用真实信息替换：

```markdown
**作者一, Zimu Yu, 作者三.**  
*论文完整标题.*  
会议 / 期刊，年份。  
[Paper](https://实际论文链接) · [Code](https://实际代码链接)
```

没有公开论文或代码链接时，删掉相应链接，不要保留示例地址。

## 上传 PDF 简历

将新版简历直接替换为 `assets/files/Zimu_Yu_CV.pdf`。CV 页面会自动嵌入并展示这份 PDF，不需要把简历正文改写成 Markdown。

## 添加资源

在 `_pages/resources.md` 的相应分类下面新增：

```markdown
- [资源名称](https://实际链接) — 一句话说明。
```

## 新增栏目

在 `_pages/` 新建 Markdown 文件，例如 `notes.md`：

```markdown
---
title: "Notes"
permalink: /notes/
---

这里写正文。
```

然后在 `_data/navigation.yml` 的 `main:` 列表末尾添加：

```yaml
  - title: "Notes"
    url: /notes/
```

## GitHub Pages

仓库 Settings → Pages → Build and deployment，选择 **Deploy from a branch**，分支 **main**，目录 **/(root)**。页面地址为 https://zimu-yu.github.io 。如果已有发布配置，保留原配置即可。

## 样式文件

`_layouts/single.html` 是 AcademicPages 风格的共用页面布局，`assets/css/site.css` 控制字体、颜色、栅格、顶部导航、作者侧栏和手机适配。一般填内容不需要修改它们。本地布局优先于远程主题布局。

原有论文状态与个人信息按仓库内容保留，后续请按最新情况更新。


## 当前页面结构

- `index.md` 是唯一的首页，包含完整个人介绍。
- `_pages/about.md` 保留为 /about/ 的介绍入口，不再与首页竞争同一地址。
- 所有内容页都有独立描述；sitemap.xml 自动收集页面，robots.txt 指向站点地图。
- CV 页面直接嵌入 `assets/files/Zimu_Yu_CV.pdf`，并在浏览器不支持内嵌时显示 PDF 链接。
- 日期、论文状态与研究经历来自现有简历及仓库，请在情况变化时更新。

## 发布与验证

`jekyll-gh-pages.yml` 负责 main 分支的正式构建和发布，并支持手动运行。
`pages.yml` 仅检查 Pull Request，不再重复发布。

使用这套自定义发布流程时，恢复账号后将 Settings → Pages → Source 设为 **GitHub Actions**，
然后在 Actions 中手动运行 “Deploy Jekyll with GitHub Pages dependencies preinstalled”。
必须等部署成功后，公开网站才可访问。账号限制不由这些代码解除。

## 搜索引擎

公开访问恢复后，可在 Google Search Console 验证网站并提交
`https://zimu-yu.github.io/sitemap.xml`。有站点地图不代表一定或立即被收录。

## 内容依据

教育、研究经历和技能由已有 Zimu_Yu_CV.tex 整理；论文与审稿状态沿用仓库资料。
未补造论文录用、实验指标、获奖、项目截图或预印本链接。
