# Slides

[slides.aisaka.cc](https://slides.aisaka.cc/) 的幻灯片目录。首页列出已发布的演示，每份演示使用独立地址，方便后续继续收录。

- `index.html`：响应式目录页，纯 HTML/CSS，无构建步骤。
- `amazon.html`：《消失的绿色》的网页演示，保留原线上版本及其资源引用。
- `amazon.md`、`eco.md`：Marp 源稿；`eco.md` 仍缺少配图，暂未收录到公开目录。
- `fonts/`：目录页使用的自托管 Barlow Condensed 字体及 SIL 许可证。

## 添加演示

1. 将完整演示导出为 HTML，使用独立文件名，例如 `topic.html`。图片等相对路径资源要一并上传，并避免与现有资源重名。
2. 在 `index.html` 的 `.collection` 中复制一张 `.deck` 卡片，更新标题、简介、页数、封面文字和链接。卡片数量按实际内容填写。
3. 在 Chrome 检查目录页的桌面和手机布局，打开演示确认翻页及图片正常。
4. 提交并推送 GitHub，然后将本次改动的静态文件同步到服务器 `/var/www/marp_slides/`。不需要修改 Caddy 或重启服务。

原本访问根路径会直接打开《消失的绿色》；现在先显示目录，演示固定入口为 `/amazon.html`。原稿中的根域名链接及二维码会进入目录页。
