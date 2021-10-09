teedoc 网站模板
=====

**中文 README | [English README](./README.md)**

此模板使用于 teedoc: [teedoc.neucrack.com](https://teedoc.neucrack.com/) 或 [teedoc.github.io](https://teedoc.github.io) learn more


## 快速开始

* 安装 python3

`Windows` 或 `macOS`, 从 [python.org](https://www.python.org/downloads/) 下载安装包安装

`Linux`, 如 `Ubuntu`:

```
sudo apt install python3 python3-pip
```

* 安装 teedoc

这条命令会 **安装 teedoc 主程序**

```
pip3 install teedoc
```

* 初始化文档

```
mkdir my_site
cd my_site
teedoc init
```

或者

```
teedoc -d my_site init
```

* 安装插件

这条命令会 **安装文档需要的插件**(在`site_config.json`里设置)

```
cd my_site
teedoc install
```

* 构建（`build`） 或者 预览（`serve`）

```
teedoc serve
```

然后浏览器访问 [http://127.0.0.1:2333](http://127.0.0.1:2333)

如果只需要构建生成网页:

```
teedoc build
```



## 几分钟内在 github pages 服务上创建你的网站


### 基于模板创建仓库

* 访问 [https://github.com/teedoc/template](https://github.com/teedoc/template) or [https://github.com/teedoc/teedoc.github.io](https://github.com/teedoc/teedoc.github.io)， 点击 `Use this template`

![github use template](./assets/github_use_template.jpg)


* 设置新仓库的名字为`用户名或者组织名.github.io`,  选择公开仓库, 然后确认提交
![create repo](./assets/create_repo.jpg)

> 之后使用`git clone 你的仓库地址`就可以克隆到本地了

### 设置 pages 服务

* 等待自动构建生成新的分支`gh-pages`, 可以点击 `Actions` 栏目查看自动构建的进度, 如果有绿色的勾勾出现了就代表可以了, 如果出现了红色的叉叉则是构建失败了, 哪里出了什么问题, 可以按照下面的截图方法点进去查看日志(提交问题必须要日志截图)并提交 [issue](https://github.com/teedoc/teedoc.github.io/issues/new) 反馈

![action status](./assets/action_status.jpg)

如果有错误, 可以按照下图点进去查看错误日志:
![error0](./assets/action_error.jpg)
![error](./assets/action_error_log.jpg)

* 设置仓库的 `pages` 服务, 选择`gh-pages`分支, 如果没有这个分支, 则是上一步还没进行完或者出错了,可以查看问题提交 [issue](https://github.com/teedoc/teedoc.github.io/issues/new) 反馈
![pages](./assets/pages_settings.jpg)

* 然后访问 `用户名或者组织名.github.io`, 就会发现有网页啦, 内容和`teedoc.github.io`的一模一样!




