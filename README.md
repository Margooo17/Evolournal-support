# Evolournal 技术支持网站

这是 Evolournal iOS 应用的技术支持网站，用于 App Store Connect 提交审核时的技术支持 URL。

## 部署方式

### 方式1：GitHub Pages（推荐）

1. **创建 GitHub 仓库**：
   ```bash
   # 在 GitHub 上创建一个新仓库，例如：evolournal-support
   ```

2. **上传文件**：
   ```bash
   git init
   git add .
   git commit -m "Add support website"
   git branch -M main
   git remote add origin https://github.com/你的用户名/evolournal-support.git
   git push -u origin main
   ```

3. **启用 GitHub Pages**：
   - 进入仓库设置 → Pages
   - Source 选择 "Deploy from a branch"
   - Branch 选择 "main"
   - 文件夹选择 "/ (root)"
   - 点击 Save

4. **获取网址**：
   - 网址格式：`https://你的用户名.github.io/evolournal-support/`

### 方式2：Netlify

1. 访问 [netlify.com](https://netlify.com)
2. 注册账号并登录
3. 点击 "Add new site" → "Deploy manually"
4. 将 `support-website` 文件夹拖拽到部署区域
5. 获得免费的 `.netlify.app` 域名

### 方式3：Vercel

1. 访问 [vercel.com](https://vercel.com)
2. 注册账号并登录
3. 点击 "New Project"
4. 导入 GitHub 仓库或直接上传文件
5. 获得免费的 `.vercel.app` 域名

## 自定义内容

在 `index.html` 中，你可以修改以下内容：

- **应用名称**：将 "Evolournal" 替换为你的应用名称
- **联系邮箱**：将 `support@evolournal.app` 替换为你的邮箱
- **应用描述**：修改应用介绍和功能描述
- **常见问题**：根据你的应用特点添加或修改 FAQ
- **颜色主题**：修改 CSS 中的颜色值以匹配你的应用主题

## 注意事项

1. **邮箱地址**：确保联系邮箱是真实有效的，Apple 可能会验证
2. **内容准确性**：确保网站内容与你的应用功能一致
3. **响应式设计**：网站已适配移动设备，无需额外修改
4. **HTTPS**：上述所有平台都提供免费的 HTTPS，满足 App Store 要求

## App Store Connect 填写

部署完成后，在 App Store Connect 的技术支持 URL 字段中填入你的网站地址，例如：
- `https://你的用户名.github.io/evolournal-support/`
- `https://你的项目名.netlify.app/`
- `https://你的项目名.vercel.app/`

## 维护建议

- 定期检查网站是否正常访问
- 及时回复用户通过邮箱发送的技术支持请求
- 根据用户反馈更新常见问题解答
- 在应用更新时同步更新网站内容 