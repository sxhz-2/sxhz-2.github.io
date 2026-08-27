# 外研版高中英语单词背诵 · 部署说明

这是一个**单文件静态网站**：`index.html` 已内置全部数据（342 对 / 103 错 / 96 错词），无需构建。

## 快速部署（3 步，全程网页操作）

详见 `guide.html`（打开照着做），要点：

1. **清空仓库 + 上传**：把 `index.html`、`guide.html`、`README.md` 上传到你的 GitHub 仓库
2. **开启 Pages**：Settings → Pages → Source 选 `Deploy from a branch` → Branch `main` / `/(root)` → Save
3. **验证**：访问 `https://你的用户名.github.io/` 显示统计即成功

## 文件说明

- `index.html` —— 网站本体（预构建，数据全在内）
- `guide.html` —— 部署指引（手机/电脑自适应，就 3 步）
- `README.md` —— 本说明
- `.nojekyll` —— 让 GitHub Pages 正常渲染（纯静态站点标配）

## 以后更新数据

改 `index.html` → 网页上传覆盖同名文件 → 约 30 秒自动上线。零命令行。

## 可选：多端同步（Supabase）

如需多设备数据同步，见 App 内「同步设置」面板 + `supabase/migrations.sql`（需自行建 Supabase 项目）。
这是可选功能，不影响网站上线。
