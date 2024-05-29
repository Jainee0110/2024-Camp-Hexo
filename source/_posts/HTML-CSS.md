---
title: HTML/CSS
date: 2024-05-29 16:13:28
tags: 
- HTML
- CSS
- Frontend

---

## 🏅 圖片空隙處理

圖片預設下方會有 2 ~ 3px 空隙，參考[此文章](https://tzuhui.github.io/2020/01/08/HTML/html-img-blank/)了解原理。

</br>

## 🏅 box-sizing

### content-box

預設值，只包括內容本身的width、height。
>舉例：
當有一個 box 設定 `width: 30px; height: 20px; border: 10px solid black;`
則此 box 總寬高：寬度: 50px, 高度: 40px

### border-box

除了內容本身的width、height ，還包括border、padding
>舉例：
當有一個 box 設定 `width: 30px; height: 20px; border: 10px solid black; box-sizing: border-box;`
則此 box 總寬高：寬度: 30px, 高度: 20px

</br>

## 🏅 [Material Icons](https://fonts.google.com/icons?icon.set=Material+Icons&icon.style=Filled)

</br>

在HTML `<head>` 內加入下方CDN，**載入 Material Icon**

```html
<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
```

將 **Icon font** 中第一個區塊程式碼貼至 HTML 區塊內
> [Material Icons 載入範例](https://codepen.io/Jainee0110/pen/gOJOPoz)

</br>

## 🏅 [Google Font](https://fonts.google.com/)

</br>

> 建議不要使用中文設定（`font-family: "微軟正黑體"`）
> 字型中間如有空格需使用引號 (`font-family: "Microsoft JhengHei"` )

### 載入方式

`<link>`：將程式碼貼到 HTML `<head>` 內

```html
<head>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Castoro:ital@0;1&display=swap" rel="stylesheet">
  <link href="style.css"> <!-- 自定義的 CSS 檔 -->
</head>
```

`@import`：在 CSS 最上方加入

```css
@import url('https://fonts.googleapis.com/css2?family=Castoro:ital@0;1&display=swap')
```
