打包为 PWA 的说明

1) 本地预览（推荐）
- 安装依赖：npm install
- 启动服务：npm run serve
- 在手机或桌面浏览器访问：http://<你的电脑局域网IP>:8765/装备洗练模拟器.html
- 在浏览器菜单选择“添加到主屏幕”即可将其作为 PWA 使用（离线时可用）。

2) 生成可分享的 ZIP 包
- 运行：npm run build-zip
- 将生成的 wx-refine-simulator-pwa.zip 文件发送到手机，解压后在浏览器打开 index.html（或 装备洗练模拟器.html）。

3) 注意事项
- 若要在局域网访问，请确保防火墙允许 8765 端口。
- iOS Safari 对 PWA 支持有限，Service Worker 在某些版本上可能不完全生效，但仍可以通过“添加到主屏幕”安装离线页面。
- 若希望发布到公开域名，直接将文件夹上传到静态托管（GitHub Pages、Netlify、Vercel等）即可。