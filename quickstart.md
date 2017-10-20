# 快速开始

我们的故事将从获取代码开始

```bash
git clone https://github.com/Moechain/Moechain.git
```

## 安装

如果在你的计算机中已经安装过Node.js的话，那么事情将会变得非常简单

```bash
cd Moechain
npm i
```

## 启动

```bash
npm start 
```
然后萌链会默认监听2333端口。

如果你想自定义监听端口，可以修改根目录下`config.json`中`port`的值。

当然，你也可以在终端中修改就像这样：

```bash
## for Linux
PORT=3300 node index.js
## or 
export PORT=3300

## for windows

set PORT=3300
## and
node index.js
```
如果不出意外的话，在控制台上将会有一头牛在向你问好，就像这样

```bash
 _______________________________________
< Moechain is listening on port: 2333 :-) >
 ---------------------------------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
             U  ||----w |
                ||     ||
```

> 接下来，萌链的API接口将为您呈现
