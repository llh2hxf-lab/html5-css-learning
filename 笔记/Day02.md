# Day 2：浏览器工作原理 + HTML 基础

**日期**：2026-03-03

---

## 一、浏览器渲染流程

浏览器打开网页的4个步骤：

```
1. 请求 → 发起 HTTP 请求获取 HTML
2. 解析 → 解析 HTML 生成 DOM 树
3. 渲染 → 解析 CSS 生成 CSSOM，两者合并成渲染树
4. 绘制 → 根据渲染树布局并绘制到屏幕
```

### 关键概念

- **DOM**：文档对象模型，HTML 的树形结构
- **CSSOM**：CSS 对象模型，样式规则的树形结构
- **渲染树**：DOM + CSSOM 合并后的可视化树

---

## 二、HTML 常用标签

### 块级元素（占一行）
```html
<div>大容器</div>
<p>段落</p>
<h1>标题</h1>
<ul>列表</ul>
```

### 行内元素（不占一行）
```html
<span>小容器</span>
<a href="#">链接</a>
<strong>加粗</strong>
<em>斜体</em>
```

### 语义化标签（HTML5 新增）
```html
<header>头部</header>
<nav>导航</nav>
<main>主要内容</main>
<article>文章</article>
<section>章节</section>
<footer>底部</footer>
```

---

## 三、HTML 标签嵌套规则

```html
<!-- 正确 -->
<div>
    <p>段落 inside div</p>
</div>

<!-- 错误：p 不能嵌套块级 -->
<p>
    <div>错误！</div>
</p>
```

---

## 今日实战代码

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>Day 2 练习</title>
    <style>
        body { font-family: sans-serif; }
        .header { background: #333; color: #fff; padding: 20px; }
        .nav a { color: #fff; margin-right: 15px; }
        .content { padding: 20px; }
        .footer { background: #eee; padding: 10px; text-align: center; }
    </style>
</head>
<body>
    <header class="header">
        <h1>我的网站</h1>
        <nav class="nav">
            <a href="#">首页</a>
            <a href="#">关于</a>
        </nav>
    </header>
    <main class="content">
        <section>
            <h2>欢迎</h2>
            <p>这是我的<strong>第一个网页</strong>！</p>
        </section>
    </main>
    <footer class="footer">
        &copy; 2026 我的网站
    </footer>
</body>
</html>
```

---

## 明日预告

Day 3：HTML 文本与链接
