# Zimu Yu · 个人学术主页

参考 Catchxu 的学术主页结构：顶部导航、左侧个人资料、右侧正文。采用 Jekyll，内容使用 Markdown。保留原有研究与论文信息。

## 以后只需改这些文件

| 想修改的内容 | 文件 |
| --- | --- |
| 名字、个人简介、所在地、邮箱、学术链接 | `_config.yml` 中的 `author` |
| 首页介绍、研究兴趣、动态 | `_pages/about.md` |
| 论文列表 | `_pages/publications.md` |
| 项目与研究 | `_pages/research.md` |
| 简历页面 | `_pages/cv.md` |
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

将文件上传到 `assets/files/Zimu_Yu_CV.pdf`，再把下面这一行加到 `_pages/cv.md`：

```markdown
[Download CV (PDF)](/assets/files/Zimu_Yu_CV.pdf)
```

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

`_layouts/single.html` 是共用页面布局，`assets/css/site.css` 控制字体、颜色、间距和手机适配。一般填内容不需要修改它们。现有 Minimal Mistakes 主题配置和插件保持不变；本地布局优先于主题布局。

原有论文状态与个人信息按仓库内容保留，后续请按最新情况更新。
