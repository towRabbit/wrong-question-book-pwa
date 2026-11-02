# 魔法学院 PWA

个人错题修炼手册 PWA，可通过 iPhone Safari 添加到主屏幕并离线使用。

## 数据存储

- 错题、分类、复习记录和图片保存在浏览器 IndexedDB。
- 每次新增、删除或修改后自动保存到本机。
- “导出到文件”通过 iOS 分享面板生成 JSON 备份，可保存到“文件”App或 iCloud Drive。
- “导入 JSON”可从文件恢复完整数据。
- 页面代码由 Service Worker 缓存，可在离线状态打开。
- 删除主屏幕应用或清理 Safari 网站数据可能导致本机数据丢失，应保留 JSON 备份。

## GitHub Pages

本项目通过 GitHub Pages 发布，入口文件为根目录下的 `index.html`。

## 本地预览

Service Worker 需要通过 HTTP 或 HTTPS 访问，可直接使用：

```bash
python3 -m http.server 8000
```

然后打开 `http://localhost:8000/`。
