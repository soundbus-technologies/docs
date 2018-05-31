# GitBook 使用方法

## 全局安装 GitBook

在这之前，你需要安装 [NodeJS](https://nodejs.org)

```sh
npm install -g gitbook-cli
```

## Clone 项目到本地

```sh
git clone https://github.com/soundbus-technologies/docs
```

## 初始化项目并安装插件

```
cd docs
gitbook init
gitbook install ./
```

## 生成静态文件

```sh
# 默认会生成 _book 文件夹，所生成的静态文件夹会存放在这里
gitbook build
```

## 本地预览

```sh
gitbook serve
```

> 浏览器访问 `http://localhost:4000`