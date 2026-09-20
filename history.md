# 修改历史

## 2026-09-20 — 创建 CleanSketch 静态官网

### 需求
根据 `pure-draw` 分支，在 Android 工程上一层目录新建静态网站，覆盖应用功能介绍、服务条款和隐私政策，并推送到 GitHub。

### 方案
1. 新建独立仓库项目 `cleansketch`（与 App 内已写死的 `https://xcat-hub.github.io/cleansketch/` 对齐）。
2. 用 Astro 静态站，结构对齐组织内 Sketch AI 官网：首页功能介绍 + `PRIVACY_POLICY.html` + `TERMS_OF_SERVICE.html`。
3. 法律文案按当前产品写：无 AI、终身一次性 Pro、开屏/激励广告、Google 登录与 Drive app-data 备份、Play Billing（不用 RevenueCat）。
4. 公开仓库 + GitHub Actions 发布 `gh-pages`。

### 修改文件
- 本仓库全部站点文件
- `history.md`
