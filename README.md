<div align="center">

<img src="./assets/logo.png" alt="MSQY's Homepage" width="128"/>

<h1>MSQY's Homepage</h1>

![最后更新](https://img.shields.io/github/last-commit/MSQY-H/homepage?label=最后更新&color=blueviolet)
![提交数](https://img.shields.io/github/commit-activity/m/MSQY-H/homepage?label=提交数&color=red)
![仓库大小](https://img.shields.io/github/repo-size/MSQY-H/homepage?label=仓库大小&color=green)
![主要语言](https://img.shields.io/github/languages/top/MSQY-H/homepage?color=blue)
![许可证](https://img.shields.io/github/license/MSQY-H/homepage?label=许可证&color=lightgrey)
[![部署](https://img.shields.io/badge/部署于-GitHub%20Pages-brightgreen)](https://msqy-h.github.io/homepage/)

</div>

> [!WARNING]
> 本项目主要代码由 AI 生成，未经专业测试，可能存在未发现的 bug。

## 项目简介

这是 MSQY 的 Homepage，可用作个人主页、个人介绍页，欢迎大家 fork 使用！

## 技术栈

本项目采用**单 HTML 文件**，内嵌 **CSS** 与 **JS** 代码，所有依赖均采用 **CDN** 方式引入，无需额外安装。

## 功能特性

- [x] 基于原生 JS，十分轻量
- [x] 流畅的动画
- [x] 支持亮色、暗色模式
- [x] 支持展示个人站点、GitHub 贡献、GitHub 项目、博客文章、最近听歌
- [x] 响应式设计

## 项目结构

``` 
homepage/
├── assets/    # README 资源文件
│   └── logo.png    # 项目 logo
├── .nojekyll    # 让 GitHub Pages 忽略 jekyll 构建
├── LICENSE    # 许可证
├── README.md    # README 文件
├── favicon.ico    # 网站图标
├── index.html    # 主文件
└── sitemap.xml    # sitemap 文件
```

## 使用方法

### 1. 修改个人信息

根据需要修改 `<head>` 部分。

主要配置项位于 `CONFIG` 变量处：

``` html
    <script>
        const CONFIG = {
        // 配置项
        };
    // 其他代码
    </script>
```

根据需要修改即可

### 2. 预览并检查信息

可以直接使用 Chrome 或 Microsoft Edge 浏览器打开 `index.html` 预览。

或者可以使用静态文件服务器的包启动

``` bash
npx serve
```

请一定要检查清楚信息是否全部修改完毕！

### 3. 部署

#### GitHub Pages

将本项目 fork 到你的帐号下，提交你进行的更改。

打开你的项目，选择 `Settings` > `Pages` > `Build and deployment` > `Source` > `Deploy from a branch`，在下方的 `Branch` 处确认分支为 `main` 或你自己的分支，根目录为 `/`，点击 `Save` 即可。

你现在应该就可以在 `https://你的用户名.github.io/你的项目名` 看到你的个人主页了。

#### Cloudflare Pages

登录到 Cloudflare Dashboard，选择 `计算` > `Workers 和 Pages` > `创建应用程序`，找到下面的 `想要开始使用 Pages？`，点击 `开始使用`，选择 `拖放文件`，填入项目名称，上传项目的整个文件夹，点击 `部署站点即可`

## 许可证

本项目使用 [MIT License](https://opensource.org/license/MIT) 进行许可。使用时请遵守 MIT License 的相关规定。