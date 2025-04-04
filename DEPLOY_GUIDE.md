# GitHub Pages 部署指南

本指南将帮助你将网站部署到GitHub Pages上。

## 步骤1：创建GitHub仓库

1. 登录你的GitHub账户
2. 点击右上角的"+"按钮，选择"New repository"
3. 输入仓库名称，建议使用：`whattodo-website`
4. 可以添加描述（可选）
5. 保持仓库为Public（这样GitHub Pages才能免费使用）
6. 不要勾选"Initialize this repository with a README"，因为我们已经有了本地仓库
7. 点击"Create repository"

## 步骤2：连接本地仓库到GitHub

在终端中执行以下命令（将`YOUR_USERNAME`替换为你的GitHub用户名）：

```bash
git remote add origin https://github.com/YOUR_USERNAME/whattodo-website.git
git branch -M main
git push -u origin main
```

## 步骤3：启用GitHub Pages

1. 在GitHub仓库页面，点击"Settings"
2. 在左侧菜单中，找到并点击"Pages"
3. 在"Source"部分，选择"Deploy from a branch"
4. 在"Branch"下拉菜单中，选择"main"，文件夹选择"/ (root)"
5. 点击"Save"

## 步骤4：访问你的网站

启用GitHub Pages后，GitHub会开始构建你的网站。几分钟后，你将看到一条消息，显示你的网站已发布，并提供网站URL。

通常URL格式为：`https://YOUR_USERNAME.github.io/whattodo-website/`

## 注意事项

- 每次你想更新网站内容，只需修改本地文件，然后执行：
  ```bash
  git add .
  git commit -m "更新内容描述"
  git push
  ```

- GitHub Pages可能需要几分钟时间来更新你的更改
- 如果你想使用自定义域名，可以在GitHub Pages设置中配置