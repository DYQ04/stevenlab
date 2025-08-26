# StevenLab Pages Starter

这是一个用于 GitHub Pages 的最小可用网站模板：

- `index.html` 主页文件
- `assets/style.css` 基础样式
- `404.html` 自定义 404 页面
- `CNAME` 绑定自定义域名（已写入 `stevenlab.top`）
- `.nojekyll` 禁用 Jekyll 处理（避免忽略下划线开头的目录）

## 使用方法（最简单）
1. 在 GitHub 新建一个仓库（例如 `stevenlab`）。
2. 上传本项目中的所有文件到仓库根目录。
3. 打开仓库 **Settings → Pages**：
   - Source: 选 `Deploy from a branch`
   - Branch: 选 `main`，文件夹选 `/ (root)`，保存
4. 在 **Settings → Pages → Custom domain** 填入：`stevenlab.top`，保存（会自动为你写入 `CNAME` 文件，如果已有则跳过）
5. 在你的域名服务商（阿里云）添加解析：
   - A 记录：`@` → 185.199.108.153 / 109.153 / 110.153 / 111.153（四条）
   - CNAME：`www` → `<你的 GitHub 用户名>.github.io`
6. 回到 **Settings → Pages** 勾选 **Enforce HTTPS**。

当 DNS 生效后，访问 `https://stevenlab.top` 即可打开网站。
