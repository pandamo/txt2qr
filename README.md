# txt2qr

输入文字或链接，即时生成二维码的网页。

## 使用

直接用浏览器打开 `index.html` 即可，兼容电脑和手机端。

也可以通过 GitHub Pages 发布：仓库 Settings → Pages → Source 选择 main 分支根目录。

## 功能

- 输入后自动生成，无需点生成按钮
- 可选纠错级别（低 / 中 / 较高 / 高）
- 下载 PNG（1024×1024）
- 复制二维码图片到剪贴板
- 支持 `?text=` 参数预填内容，例如 `index.html?text=https://example.com`
- 二维码在本地生成，输入内容不上传服务器

## 技术

- 单页应用，样式内联于 `index.html`
- 二维码库为本地文件 `js/qrcode.min.js`（由 npm 包 `qrcode@1.5.4` 打包而来），页面不引用任何 CDN 上的 JS
