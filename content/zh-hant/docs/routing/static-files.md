---
title: "靜態文件"
date: 2020-04-09T10:53:41+08:00
---

```go
router.ServeFiles("/assets/*filepath", http.Dir("/path/to/assets"))
```

其將請求路徑 `/assets/*filepath` 映射到目錄 `/path/to/assets`:

- `GET /assets/css/app.css` => `/path/to/assets/css/app.css`
- `GET /assets/js/app.js` => `/path/to/assets/js/app.js`
- ...

我們也可以將 `http.FileServer` 作爲 `NotFound` 處理器, 比如 `/robots.txt`, `/favicon.ico`.

```go
router.NotFound = http.FileServer(http.Dir("public"))
```