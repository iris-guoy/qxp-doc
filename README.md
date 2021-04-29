# 全象云平台文档页面

此项目是通过Hugo框架 + Dot主题（暂定） 搭建 使用Netlify 全自动部署

全象云平台文档预览页面地址（暂定）：https://qxp-doc.netlify.app/

文档源码github地址：https://github.com/EriccReeves/qxp-doc.git

Hugo框架文档地址（中文）：https://www.gohugo.org/doc/

Dot主题文档地址（英文）：https://docs.gethugothemes.com/dot/

## 本地安装指南

请确保你已经安装了 Git命令行 与 VS Code ，还有 谷歌浏览器

> 以下步骤适用于macOS，其他系统以此类推把

### 第一步：安装Hugo

> `macOS`的`Homebrew`软件包管理器可以从[brew.sh](https://brew.sh/)安装软件包。如果您正在运行Windows等，请参阅[安装](https://gohugo.io/getting-started/installing)。

* 检查是否安装Homebrew

  ```bash
  brew -v
  ```

  若没有出现类似于一下文本信息，则需要安装Homebrew

  ```bash
  Homebrew 3.1.4
  Homebrew/homebrew-core (git revision ca88452bac; last commit 2021-04-28)
  ```

  将以下命令粘贴至终端后，等待安装完成即可

  ```bash
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  ```

* 安装Hugo

  ```bash
  brew install hugo
  ```

  要验证您的新安装，请执行以下操作：

  ```bash
  hugo version
  ```

### 第二步：管理文档项目源码

* 进入当前用户目录，克隆代码

  ```bash
  cd ~
  git clone git@github.com:EriccReeves/qxp-doc.git
  cd qxp-doc
  ```

* 获取管理代码管理权限

  * 配置git的的全局用户名与邮箱

    ```bash
    git config --global user.name "your_username"
    git config --global user.email "your_email"
    ```

  * 联系管理员添加Github仓库权限

### 第三步：启动本地项目

* 进入项目根目录，启动本地调试服务器

  ```base
  cd qxp-doc
  hugo server -D
  ```

  启动成功后访问 http://localhost:1313/ 或者 http://127.0.0.1:1313/

