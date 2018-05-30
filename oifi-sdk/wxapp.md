---
description: 微信小程序云端解析 OIFI SDK
---

# 微信小程序

## 安装

使用 NPM 管理微信小程序 OIFI SDK

```bash
npm install sound-oifi
```

## 使用

将 sound-oifi.js 直接放到微信小程序的项目中，使用 commonjs 引入

```javascript
var OIFI = require('sound-oifi')
```

如果你使用 [WePy](https://github.com/Tencent/wepy) 可以这样引入

```javascript
import OIFI from 'sound-oifi'
```

### 初始化

```javascript
var oifi = new OIFI({
  key: 'OIFI KEY',
  success: function (res) {
    // 声波解析成功后将在这里返回数据，可以在这里处理你的业务逻辑
    console.log(res)
  },
  fail: function (error) {
    console.log(error)
  }
})
```

### 开启解析

开启录音，与云端建立通讯，音频流实时上传到云端解析

```javascript
oifi.startListen()
```

### 停止解析

```javascript
oifi.stopListen()
```