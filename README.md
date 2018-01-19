# ChaZD-thinkam

简洁易用的英汉字典扩展程序，支持划词， 可自定义有道智云ID、密钥

## 一、版本介绍

如果你想体验原版的ChaZD，请选择v1.0.0，后面几个版本是我根据个人的使用情况和偏好添加了几个功能，欢迎尝试，具体信息见releases界面。

## 二、使用说明

### 2.1 下载插件


下载地址：https://github.com/codethereforam/ChaZD/releases

选择你想要的版本，下载ChaZD-thinkam.crx文件。如果你的浏览器支持使用非Web Store的插件，直接将下载的crx拖到chrome://extensions/页面。

如果不支持，将crx文件扩展名改为zip并解压，在chrome://extensions/勾选开发者模式，接着在 Chrome 设置拓展的地方，点击加载未打包的拓展。详细步骤见[chrome怎么安装非官方市场的插件？ - 小赖的回答](https://www.zhihu.com/question/24027794/answer/34500157)。

### 2.2 申请有道智云翻译服务

- 注册[有道智云](http://ai.youdao.com/)帐号并登录到控制台页面
- 创建一个翻译实例：控制台 > 自然语言翻译 > 翻译实例 > 创建翻译实例
- 创建一个应用并绑定翻译服务：控制台 > 应用管理 > 我的应用 > 创建应用 > 绑定服务
- 在插件中绑定应用——将上步骤的应用ID和应用密钥填写到插件设置页中相应的位置，如下图

![](/screenshoot/ChaZD-01.png)

ChaZD
=====

ChaZD 查字典，简洁易用的英汉字典扩展程序，支持划词哦:)
翻译结果和发音朗读由**有道翻译**驱动。

获取
-----------
+ [Chrome 网上应用商店](https://chrome.google.com/webstore/detail/chazd/nkiipedegbhbjmajlhpegcpcaacbfggp)
+ [crx 文件](https://github.com/ververcpp/ChaZD/blob/master/ChaZD.crx?raw=true)

**注**：安装扩展后，第一次使用请刷新要查词的页面，划词功能才会生效；
**注2**：非中文版Chrome浏览器的用户，如出现插件弹出窗口字体无法正常显示的情况，麻烦请更改浏览器的最小字号为12px
（具体步骤: settings-->show advanced settings-->Web content中的Customize fonts... -->Minimum font     size将最小字号改为12px）。

主要功能
-----------
+ 支持在线英汉互译
+ 提供英文单词和语句的英音、美音真人发音朗读
+ 支持网页内英文划词翻译
+ 可通过快捷键（Ctrl+Shift+F）快速启动词典扩展，也可以自定义快捷键
+ 可设置开启与关闭划词功能，并可选择划词结果的显示位置

截图
-----------
![Screenshoot 1](/screenshoot/screenshoot1.jpg)
---
![Screenshoot 2](/screenshoot/screenshoot4.png)

修改代码及部署
-----------

确保你已经安装了[Node.js](http://nodejs.org/)以及[grunt-cli](https://github.com/gruntjs/grunt-cli),

下载代码并部署
```shell
git clone https://github.com/ververcpp/ChaZD.git
cd ChaZD && npm install   #安装部署依赖的包
grunt                     #部署代码
```

进入Chrome的扩展程序设置页面，点击“加载正在开发的扩展程序”，选择ChaZD目录

可以使用`grunt watch`实时更新修改的js、css文件并部署，
每次修改代码之后直接在浏览器的扩展程序设置页面重新加载ChaZD即可

-----------
部分功能设计借鉴于[TransIt](https://github.com/GDG-Xian/crx-transit)

源码完全开放，欢迎Star、Fork、提交BUG，并提出您宝贵的意见与建议。
