# 我的错题本 PWA

个人错题本 PWA，可通过 iPhone Safari 添加到主屏幕并离线使用。

## 数据存储

- 错题数据保存在浏览器 IndexedDB。
- 每次新增、删除或修改后自动保存。
- 页面代码由 Service Worker 缓存，可在离线状态打开。
- 删除主屏幕应用或清理 Safari 网站数据可能导致错题丢失。

## GitHub Pages

本项目通过 GitHub Pages 发布，入口文件为根目录下的 `index.html`。

## 本地预览

Service Worker 需要通过 HTTP 或 HTTPS 访问，可直接使用：

```bash
python3 -m http.server 8000
```

然后打开 `http://localhost:8000/`。
