# Day 1：HTTP/TCP 基础 + HTML 概述

**日期**：2026-03-03

---

## 一、HTTP 请求响应原理

### 什么是 HTTP？
- 超文本传输协议，浏览器和服务器之间的"对话语言"
- 请求-响应模式：客户端发请求 → 服务器返回响应

### HTTP 请求结构
```
请求行    GET /index.html HTTP/1.1
请求头    Host: example.com
         User-Agent: Chrome...
空行
请求体    (POST 数据)
```

### HTTP 响应结构
```
状态行    HTTP/1.1 200 OK
响应头    Content-Type: text/html
空行
响应体    <html>...页面内容...</html>
```

---

## 二、TCP 三次握手

建立连接的三步：
1. **SYN**：客户端 → 服务器 "我要连接"
2. **SYN-ACK**：服务器 → 客户端 "好的，收到"
3. **ACK**：客户端 → 服务器 "那我们开始吧"

**四次挥手**：断开连接（了解即可）

---

## 三、URL 与 DNS

### URL 格式
```
https://www.example.com:443/path?name=value#anchor
 协议   主机名          端口  路径      查询   锚点
```

### DNS
域名→IP 地址的"电话簿"

---

## 四、HTML 基本结构

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>页面标题</title>
</head>
<body>
    <h1>Hello World</h1>
    <p>这是一个段落</p>
</body>
</html>
```

---

## 今日实战

在本地创建 `index.html` 文件，复制上面的代码，用浏览器打开。

---

## 明日预告

Day 2：浏览器工作原理 + HTML 基础
