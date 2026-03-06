# gitblog

一个最小可用的静态博客仓库，使用 **GitHub Pages** 自动部署。

## 部署方式
- 分支：`main`
- 触发：push 到 `main` 后自动部署（GitHub Actions）

## 本地预览
直接双击 `index.html` 或用任意静态服务器打开。

## 首次上线步骤
1. 在 GitHub 创建空仓库（建议名：`gitblog`）
2. 绑定远程并推送：

```bash
git remote add origin git@github.com:niezefeng/gitblog.git
git add .
git commit -m "init: github pages blog"
git push -u origin main
```

3. 到 GitHub 仓库设置开启 Pages（若未自动开启）：
   - Settings → Pages → Build and deployment → Source 选择 **GitHub Actions**

完成后访问：
- `https://niezefeng.github.io/gitblog/`

如果你把仓库名改成 `<user>.github.io`，则地址会变成根域名。
