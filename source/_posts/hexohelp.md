---
title: 记一次使用Hexo
author: RemMai
avatar: 'https://cdn.jsdelivr.net/gh/remmai/cdn@1.0/img/custom/avatar.jpg'
authorLink: 'https://blog.RemMai.cn'
authorAbout: 一个不怎么幸运的男孩~
authorDesc: 一个不怎么幸运的男孩~
comments: true
date: 2020-04-21 01:16:02
tags: 经验历程
keywords:
description:
photos:
    - http://p8.qhimg.com/bdr/__100/t01e467a69210d5812a.jpg
---
前言：由于是第一次使用第二台设备使用Hexo，所以有了这次笔记。

- 使用Git将仓库中的东西拉取下来。
- 使用`npm install` 安装需要的包。

这个时候，我们的基本环境已经配置好了，使用`hexo s`将服务跑起来即可。

# Hexo 指令

> 怕自己忘记才记录的。（个人常用）[官方文档](https://hexo.io/zh-cn/docs/commands.html)

## new

```
$ hexo new [layout] <title>
```

新建一篇文章。如果没有设置 `layout` 的话，默认使用 [_config.yml](https://hexo.io/zh-cn/docs/configuration) 中的 `default_layout` 参数代替。如果标题包含空格的话，请使用引号括起来。

```shell
$ hexo new "post title with whitespace"
```

| 参数              | 描述                                          |
| :---------------- | :-------------------------------------------- |
| `-p`, `--path`    | 自定义新文章的路径                            |
| `-r`, `--replace` | 如果存在同名文章，将其替换                    |
| `-s`, `--slug`    | 文章的 Slug，作为新文章的文件名和发布后的 URL |

## server

```
$ hexo server
```

启动服务器。默认情况下，访问网址为： `http://localhost:4000/`。

| 选项             | 描述                           |
| :--------------- | :----------------------------- |
| `-p`, `--port`   | 重设端口                       |
| `-s`, `--static` | 只使用静态文件                 |
| `-l`, `--log`    | 启动日记记录，使用覆盖记录格式 |