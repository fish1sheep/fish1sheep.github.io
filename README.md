# 🤖 机器人技术博客 (My Robotics Blog)

[][gem] 
[][mit]

这是一个基于 [GitHub Pages](https://pages.github.com/) 搭建的个人博客，主要用于记录和分享 **机器人（Robotics）** 相关的技术文章、开发日志和项目心得。

本博客使用了 [**Chirpy Starter**](https://github.com/cotes2020/chirpy-starter) 模板进行构建。

-----

## 📌 为什么基于 Starter 模板构建？

如果直接通过 RubyGems.org 安装 Chirpy 主题，Jekyll 只能读取一小部分主题文件（如 `_data`、`_layouts` 等），这会导致很多开箱即用的高级功能无法正常显示。

为了完整解锁 Chirpy 的所有特性，本仓库保留了 Starter 模板中预配置的关键文件：

```shell
.
├── _config.yml   # 博客的核心配置文件
├── _plugins      # 插件目录
├── _tabs         # 侧边栏标签（如关于、归档等）
└── index.html    # 博客首页
```

通过这个模板，我们可以绕过繁琐的配置，直接专注在机器人内容的创作上！

-----

## 📖 参考与文档

  * **博客主题文档**：关于如何写文章、插入图片或公式，请参考 [Chirpy Wiki](https://github.com/cotes2020/jekyll-theme-chirpy/wiki)。
  * **持续集成**：仓库已内置 [CD][CD] 工作流，推送到 `master`/`main` 分支后会自动构建并部署到 GitHub Pages。

## 📄 开源协议

本仓库基于 [MIT][mit] 协议开源。

[gem]: https://www.google.com/search?q=%5Bhttps://rubygems.org/gems/jekyll-theme-chirpy%5D\(https://rubygems.org/gems/jekyll-theme-chirpy\)
[mit]: https://www.google.com/search?q=%5Bhttps://github.com/cotes2020/chirpy-starter/blob/master/LICENSE%5D\(https://github.com/cotes2020/chirpy-starter/blob/master/LICENSE\)
[cd]: https://www.google.com/search?q=%5Bhttps://en.wikipedia.org/wiki/Continuous_deployment%5D\(https://en.wikipedia.org/wiki/Continuous_deployment\)
