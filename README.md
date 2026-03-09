# 找牛牛 🐄

在微信中打开此游戏的步骤：

## 方法一：部署到静态托管（推荐）

1. 将整个 `minesweeper` 文件夹内的文件（`index.html`、`mine-icon.png`）上传到任意静态网站托管服务，例如：
   - **GitHub Pages**：创建仓库，上传文件，在 Settings → Pages 中启用
   - **Vercel / Netlify**：拖拽文件夹即可部署
   - **腾讯云 COS / 阿里云 OSS**：开启静态网站托管，上传后获得访问地址

2. 获得形如 `https://xxx.com/` 的访问地址后，将该链接发送到微信，点击即可在微信内置浏览器中打开游戏。

## 方法二：本地预览

```bash
cd minesweeper
python -m http.server 8080
```

浏览器访问 `http://localhost:8080` 预览。注意：微信无法直接打开本地地址，需部署到公网才能分享到微信。
