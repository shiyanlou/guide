# 实验楼软件库使用方法

本文档介绍向实验楼软件库提交软件的过程，让你为感兴趣的软件开通在线体验。

实验楼软件库是一个开放的软件在线体验平台，可以发现并一键体验最新的开源软件。

我们欢迎任何开源爱好者和软件作者向实验楼的软件库提交优质的软件，让更多的人能够在线快速体验。

## 提交软件的步骤

1. Fork 示例仓库并修改名称
2. 完成快速上手教程及实验环境 Dockerfile
3. 申请上线
4. 测试并上线

## 第一步：Fork 示例仓库并修改名称

进入到示例仓库 https://github.com/shiyanlou/trylab，Fork 一份成为自己的仓库。

点击 Fork 后的仓库的 `Settings`，修改 `Repository name` 下的名字为你要提交的软件的名字，例如 mysoftware，然后点击 `Rename` 按钮。

## 第二步：完成快速上手教程及实验环境 Dockerfile

在新 Fork 的仓库中，有下面几个文件：

1. doc.md：提交软件的快速上手教程，需要使用 Markdown 语法编写，如果有插入的图片，需要将图片保存到 `images/` 目录下
2. images/：保存快速上手教程中的图片
3. Dockerfile：包含软件的环境使用的 Dockerfile，软件库中的软件在线体验使用 Docker 容器的形式
4. README.md：对软件的简单介绍，至少包含软件名称，描述，License，软件主页，相关的教程资源，Dockerfile 的使用方法。

### 注意

1. `doc.md` 快速上手教程需要包含使用软件最常用功能的详细步骤，让用户可以边看边体验
2. `Dockerfile` 可以直接使用 [Docker Hub](https://hub.docker.com/explore/) 上已有的 `Dockerfile`，也可以自己编写，必须保证容器构建没有问题
3. 如果对 Markdown 语法不熟悉，可以参考 [Markdown 快速教程](https://www.shiyanlou.com/questions/764)
4. 如果对 Dockerfile 不熟悉，可以参考 [Dockerfile 教程](http://cepave.com/how-to-write-dockerfile/)


## 第三步：申请上线

点击下方的链接，创建 issue 填写你的仓库地址申请上线。

[申请上线](https://github.com/shiyanlou/guide/issues/new)

## 第四步 测试并上线

为了保证用户的体验，我们会对提交的软件和文档进行严格的审核及测试，测试中发现的问题也会给你的仓库提交 issue 或 PR。

测试通过后我们会上线到实验楼的软件库，并将该软件页面中的 `Fork on github` 及 `纠错` 关联到你的仓库。Github 仓库由你维护，更新后我们会定期更新到线上，如果有比较急的修复可以直接 [创建 issue](https://github.com/shiyanlou/guide/issues/new)。

## 联系我们

如果您对实验楼软件库和提交软件有任何疑问，可以直接在本项目创建 issue，或者邮件我们 support@shiyanlou.com
