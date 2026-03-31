---
title: GitHub Pages 博客写作教程
date: 2026-03-31 10:00:00 +0800
categories:
  - 教程
tags:
  - GitHub Pages
  - Jekyll
  - Chirpy
toc: true
comments: true
---

本博客基于 **Jekyll** 静态网站生成器，使用 **Chirpy** 主题。本教程将详细介绍如何在这里撰写博客文章。

<!-- more -->

## 一、文章存放位置

所有博客文章都存放在 `_posts/` 目录下。

## 二、文件命名规范

文件名必须遵循以下格式：

```
YYYY-MM-DD-title.md
```

示例：
- `2026-03-31-hello-world.md`
- `2026-04-15-my-second-post.md`

## 三、Frontmatter 格式

每篇文章的开头必须包含 YAML frontmatter，用于指定文章的元数据。

### 3.1 必需字段

```yaml
---
title: 文章标题
date: 2026-03-31 10:00:00 +0800
---
```

### 3.2 可选字段

```yaml
---
title: 文章标题
date: 2026-03-31 10:00:00 +0800
categories:
  - 分类1
  - 分类2
tags:
  - 标签1
  - 标签2
toc: true          # 是否显示目录（Table of Contents）
comments: true     # 是否启用评论
image: /assets/img/cover.png  # 封面图片（可选）
---
```

## 四、Markdown 语法

### 4.1 标题

```markdown
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
```

### 4.2 文字格式

```markdown
**粗体文字**
*斜体文字*
~~删除线文字~~
`行内代码`
```

效果：**粗体** *斜体* ~~删除线~~ `代码`

### 4.3 列表

**无序列表：**

```markdown
- 第一项
- 第二项
  - 嵌套项
- 第三项
```

**有序列表：**

```markdown
1. 第一步
2. 第二步
3. 第三步
```

### 4.4 链接和图片

```markdown
[链接文字](https://example.com)

![图片描述](/assets/img/example.png)
```

### 4.5 引用

```markdown
> 这是一段引用内容。
> 可以多行。
```

效果：
> 这是一段引用内容。
> 可以多行。

### 4.6 代码块

使用三个反引号包裹，并指定语言：

````markdown
```python
def hello():
    print("Hello, World!")
```
````

效果：

```python
def hello():
    print("Hello, World!")
```

常用语言标记：`python`, `javascript`, `java`, `c`, `cpp`, `bash`, `yaml`, `json`, `markdown`, `html`, `css`, `ruby`, `go`, `rust` 等。

### 4.7 表格

```markdown
| 列1 | 列2 | 列3 |
|-----|-----|-----|
| A   | B   | C   |
| D   | E   | F   |
```

效果：

| 列1 | 列2 | 列3 |
|-----|-----|-----|
| A   | B   | C   |
| D   | E   | F   |

### 4.8 分割线

```markdown
---
```

效果：

---

## 五、 Chirpy 主题特殊功能

### 5.1 目录（TOC）

在 frontmatter 中设置 `toc: true` 即可自动生成目录。

### 5.2 文章摘要

在正文中使用 `<!-- more -->` 标记，标记之前的内容将作为摘要显示在文章列表中。

### 5.3 目录跳转

使用 HTML 锚点跳转到指定章节：

```markdown
[跳转到常用配置](#常用配置)
```

### 5.4 数学公式

 Chirpy 主题支持 LaTeX 数学公式，使用 `$...$` 表示行内公式，`$$...$$` 表示独立公式块。

## 六、写作流程

1. 在 `_posts/` 目录下创建新文件，命名格式：`YYYY-MM-DD-your-title.md`
2. 编写 frontmatter
3. 撰写正文内容
4. 本地预览（如需要）
5. 推送到 GitHub 仓库
6. GitHub Pages 自动构建并发布

## 七、本地预览

如果需要在本地预览文章效果：

```bash
# 安装依赖
bundle install

# 启动本地服务器
bundle exec jekyll serve

# 访问 http://localhost:4000 查看
```

## 八、注意事项

- 所有文章必须使用 UTF-8 编码
- 图片建议放在 `assets/img/` 目录下
- 文章日期决定了发布顺序，请确保日期格式正确
- 推送到 main 分支后，GitHub Pages 会自动部署

---

如有问题，请查看 [Chirpy 主题文档](https://github.com/cotes2020/jekyll-theme-chirpy) 或提交 Issue。
