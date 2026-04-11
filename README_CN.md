<p><a href="./README.md">English</a> | <b>简体中文</b></p>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7C3AED,100:06B6D4&height=180&section=header&text=GitHub%20Profile%20%E6%A8%A1%E6%9D%BF&fontSize=42&fontAlignY=38&animation=fadeIn&fontColor=white&desc=%E6%B7%B1%E8%89%B2%E7%B3%BB%E3%80%81%E5%8A%A8%E6%80%81%E6%95%88%E6%9E%9C%E3%80%81%E5%BC%80%E7%AE%B1%E5%8D%B3%E7%94%A8&descAlignY=62&descSize=16" />

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=2000&pause=500&color=A78BFA&center=true&vCenter=true&width=620&lines=%E6%B7%B1%E7%B4%AB+%E2%86%92+%E7%94%B5%E9%9D%92+%E9%85%8D%E8%89%B2%E6%96%B9%E6%A1%88;Snake+%E5%8A%A8%E7%94%BB+%2B+3D+%E8%B4%A1%E7%8C%AE%E5%9B%BE;%E5%AE%8C%E5%85%A8%E5%8F%AF%E5%AE%9A%E5%88%B6+%7C+%E5%A4%8D%E5%88%B6%E5%8D%B3%E7%94%A8" />

<p align="center">
  <a href="./README.md"><img src="https://img.shields.io/badge/English-7C3AED?style=for-the-badge" /></a>
  <a href="#模板特点"><img src="https://img.shields.io/badge/模板特点-5B21B6?style=for-the-badge" /></a>
  <a href="#快速开始"><img src="https://img.shields.io/badge/快速开始-4338CA?style=for-the-badge" /></a>
  <a href="#actions-配置"><img src="https://img.shields.io/badge/Actions配置-0E7490?style=for-the-badge" /></a>
  <a href="#个性化定制"><img src="https://img.shields.io/badge/个性化定制-06B6D4?style=for-the-badge" /></a>
</p>

</div>

---

## ✨ 模板特点 <a id="模板特点"></a>

- **波浪横幅**：渐变色标题 + 副标题，via capsule-render
- **打字机动画**：循环显示个人标签（Fira Code 字体）
- **社交徽章**：GitHub、邮箱、ORCID、Google Scholar、小红书
- **页面访问计数**（komarev.com）+ Stars 统计
- **技能图标墙**：via skillicons.dev
- **贡献统计卡片**：三张 summary cards（tokyonight 主题）
- **Snake 贡献动画**：深色/浅色模式自适应，每天自动更新
- **贡献热力图**：profile-details 卡片 + 3D 彩虹贡献图
- **页脚波浪**：渐变动画收尾

---

## 🚀 快速开始 <a id="快速开始"></a>

### 第一步 — 创建同名仓库

当仓库名与你的 GitHub 用户名完全一致时，GitHub 会将其 `README.md` 展示为你的个人主页。

1. 打开 **github.com/new**
2. 仓库名填写你的 **GitHub 用户名**（如 `zyh3699`）
3. 设为 **Public**
4. 勾选 **Add a README file**
5. 点击 **Create repository**

### 第二步 — 复制模板

1. 打开 [`zyh3699/zyh3699`](https://github.com/zyh3699/zyh3699/blob/main/README.md)，点击 **Raw**
2. 全选 → 复制
3. 粘贴到你新仓库的 `README.md` 中
4. 将所有 `zyh3699` 替换为**你的用户名**

### 第三步 — 替换个人信息

找到以下内容并替换：

| 占位内容 | 替换为 |
|---|---|
| `zyh3699` | 你的 GitHub 用户名 |
| `zephyrzhong248@gmail.com` | 你的邮箱 |
| `0009-0003-0132-2036` | 你的 ORCID |
| `your-id`（Google Scholar） | 你的 Scholar 用户 ID |
| 小红书个人主页链接 | 你的链接（或删除该徽章）|

### 第四步 — 配置 GitHub Actions

Snake 动画和 3D 贡献图需要两个 workflow，详见下方 **[Actions 配置](#actions-配置)**。

### 第五步 — 提交并预览

提交更改后，访问 `github.com/你的用户名` 即可看到效果。

---

## ⚙️ Actions 配置 <a id="actions-配置"></a>

将 [`zyh3699/zyh3699/.github/workflows/`](https://github.com/zyh3699/zyh3699/tree/main/.github/workflows) 中的两个 workflow 文件复制到你仓库的 `.github/workflows/` 目录下。

### Snake 动画（`snake.yml`）

自动生成贡献网格 Snake 动画，推送到 `output` 分支，每天零点更新。

**配置步骤：**

1. 进入你的仓库 → **Settings** → **Actions** → **General**
2. 找到 *Workflow permissions*，选择 **Read and write permissions**
3. 保存

**首次运行：**

进入 **Actions** → `Generate Snake Animation` → **Run workflow**

生成后 SVG 路径为：
```
https://raw.githubusercontent.com/你的用户名/你的用户名/output/github-contribution-grid-snake-dark.svg
https://raw.githubusercontent.com/你的用户名/你的用户名/output/github-contribution-grid-snake.svg
```

---

### 3D 贡献图（`profile-3d.yml`）

生成 3D 动态贡献图，推送到 `main` 分支，每天 18:00 UTC 自动更新。

**需要 Personal Access Token（PAT）**

1. 打开 **github.com/settings/tokens** → **Generate new token (classic)**
2. 填写名称（如 `PROFILE_TOKEN`）
3. 勾选权限：✅ `repo`
4. 生成并**复制 Token**
5. 进入你的仓库 → **Settings** → **Secrets and variables** → **Actions** → **New repository secret**
6. 名称填 `TOKEN`，值粘贴你的 Token
7. 保存

**首次运行：**

进入 **Actions** → `3D贡献图` → **Run workflow**

生成后路径为：
```
https://raw.githubusercontent.com/你的用户名/你的用户名/main/profile-3d-contrib/profile-night-rainbow.svg
```

> ⚠️ 重要：3D 贡献图的颜色配置需要同时修改 `profile-3d-contrib/settings.json` 和 `profile-3d.yml` 中内联的 JSON，否则 workflow 运行时会用旧配置覆盖文件。

---

## 🎨 个性化定制 <a id="个性化定制"></a>

### 配色方案

模板使用**深紫 → 电青**渐变，关键颜色值：

| 用途 | 十六进制 |
|---|---|
| 主色（紫） | `#7C3AED` |
| 辅色（青） | `#06B6D4` |
| 中间过渡 | `#4E7FD4` |
| 强调色（浅紫）| `#A78BFA` |

修改配色时，需同时更新 Banner、页脚、徽章、stats 主题中的对应值。

### 打字机文案

修改 Typing SVG URL 中的 `lines=` 参数，多行用 `;` 分隔，空格用 `+` 表示。

### 技能图标

修改 skillicons.dev URL 中的 `i=` 参数：
```
https://skillicons.dev/icons?i=python,pytorch,tensorflow,docker,...&perline=9
```
完整图标列表：[skillicons.dev](https://skillicons.dev)

### 统计卡片主题

将 `theme=tokyonight` 替换为其他主题：
`dark`、`radical`、`merko`、`gruvbox`、`tokyonight`、`onedark`、`cobalt`、`synthwave`、`dracula`

### 3D 贡献图配色

同时修改 `settings.json` 和 `.github/workflows/profile-3d.yml` 中的内联 JSON：

```json
{
  "type": "rainbow",
  "backgroundColor": "#0d1117",
  "radarColor": "#7C3AED",
  "growingAnimation": true,
  "contribColors": ["#161b22", "#2D1B69", "#5B21B6", "#7C3AED", "#06B6D4"]
}
```

---

## 📄 许可协议

MIT 许可证 — 可自由使用、修改和分发。详见 [LICENSE](./LICENSE)。

<p align="center">
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-7C3AED?style=for-the-badge" alt="MIT License" />
  </a>
</p>

<p align="center"><i>如果这个模板对你有帮助，欢迎点个 ⭐ 支持一下！</i></p>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7C3AED,50:4E7FD4,100:06B6D4&height=120&section=footer&animation=twinkling" width="100%"/>
