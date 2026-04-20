# Algorithm Contest Record

Algorithm Contest Record (ACR) 是一个用于记录算法竞赛题解的个人站点。

## 站点定位

- 主要内容：Codeforces 与 AtCoder 比赛题解
- 更新方式：按比赛持续记录赛后复盘与思路总结
- 目标：沉淀可检索、可复习的解题方法库

## 目录约定

- 比赛题解统一放在 `content/post/`
- 固定页面在 `content/page/`
- 全局配置在 `config/_default/`

## 本地预览

```bash
hugo server -D
```

默认访问地址：`http://localhost:1313/`

## GitHub 自动部署

本仓库已包含 GitHub Actions 工作流：

- `.github/workflows/deploy-pages.yml`

部署方式：

1. 推送到 `main`（或 `master`）分支后自动触发构建与部署。
2. 首次使用时，在仓库 Settings -> Pages 中确认 Source 为 GitHub Actions。
3. 若主题以 submodule 方式管理，工作流会自动递归拉取 submodule。

部署地址通常为：

- `https://<your-username>.github.io/<repo-name>/`