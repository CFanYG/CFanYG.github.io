<p align="center">
    <img src="https://pic.tyzhang.top/images/2021/01/14/logo_b.png" width="100px"/>
</p>

## 如云 / hexo-theme-ruyun

一个 Hexo 个人博客主题。

基于[胡伟煌](http://www.huweihuang.com/)移植的[黄玄 Jekyll 博客主题](https://github.com/Huxpro/huxpro.github.io)修改而来。我对它进行了一些调整和新增，以便更适合我的口味。

### 🎨 修改

- **大道至简**：删除多项不必要的功能插件。
- **我的口味**：主页、文章样式的修改，更简洁直观。
- **每天皆不同**：唯一的不同，就是处处皆不同。修改文章默认头图为每日必应壁纸，增加[每日一句](https://hitokoto.cn/api)、[一诗](https://www.jinrishici.com)等 widget 插件。
- **古法传承**：主要内容的汉化。
- **早韭晚菘**：增加网易云音乐作为背景音乐模块，为你的文章、页面配一个更应景的BGM。
- **一碗米粉**：放置你自己的公众号、赞赏码等二维码。
- **备案轻松**：一键设置备案网站 ICP 备案号、公安部备案号。
- **LaTex**：增加对 LaTex 公式的渲染、正常显示。
- **社交加加**：增加知乎、哔哩哔哩和即刻社交页面展示。
- **搜索到位**：依托 [Dogedoge](https://www.dogedoge.com/) 实现站内检索功能。

### 🌈 效果

我的博客: [ztygalaxy](https://ztygalaxy.github.io)，部分插件未启用。

![demo](https://pic.tyzhang.top/images/2021/01/14/demo.png)

### 🔨 用法

在 `_config.yml` 中配置个人信息。

#### 1. 替换 Repo 信息.

```yml
deploy:
  type: git
  repository: 你的Repo名称，如ztygalaxy.github.io
  branch: master
  message: Update Content
```

#### 2. 继续客制化.

通过替换、修改 `source/img/avatar/ironman.png` 来配置头像。

或者修改它的路径：

```yml
sidebar: true    # 侧边栏开关.
sidebar-about-description: "你的个人描述"
sidebar-avatar: img/你的头像路径
```

在 `widgets` 下配置侧边栏的部件，使用 `#` 关闭。

```yml
widgets:
- featured-tags        # 标签
- short-about        # 简介
#- recent-posts        # 最新文章
#- friends-blog        # 友链
- archive            # 归档
- category            # 分类
- a-sentence        # 每日一句
- a-poem            # 每日诗句
- qrcode            # 二维码展示，/img/avatar/qrcode.png
- search            # 搜索功能
```

如果你的网站需要放置备案信息，填写 `icp`。

钢铁侠的回到顶部，可在 `css/image` 中替换。

其他样式和资源文件，可以在浏览器中检查元素到对应文件修改，例如 `layout` 文件夹下，它们的名字作用都很明了。

在 `feed` 中配置 RSS 订阅，[参数说明](https://github.com/hexojs/hexo-generator-feed#options).

#### 3. 文章撰写与参数说明

你应该非常熟悉 hexo 文章的生成撰写，也可以在给出的样例文章基础上修改，参数说明如下。

```yml
---
title:                     # 文章名称
subtitle:                # 子标题，在博文列表显示简介
date:                    # 创建日期
catalog: true            # 是否使用目录
header-img:                # 头图地址
tags:                    # 标签
toc_nav_num: true        # 是否使用目录
musicid:                 # 如果需要背景音乐，请填写其网易云id
musicauto: 1            # 是否需要自动播放，默认为1
top: 0                    # 是否需要置顶
---
```

### 👦 相关

[胡伟煌的博客](http://www.huweihuang.com/)    [黄玄的博客]( http://huangxuan.me/ )    [张天宇的博客](https://ztygalaxy.github.io)

相关阅读：[Hexo是怎么工作的](http://coderunthings.com/2017/08/20/howhexoworks/)