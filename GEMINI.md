# 出海独立站集群全局开发规范 (Workspace Guidelines)

本规范适用于工作区内所有出海站点（如游戏 Wiki、出海工具站等）的代码生成与前端重构，所有后续开发任务必须严格遵守。

---

## 🎨 一、 UI 视觉与图标规范 (Icon & Visual Standards) 【强制执行】

### 1. 原生 Emoji 禁用规则
* **【严禁】** 在任何页面的 **导航栏（Navbar）、核心 Hero 区、特性卡片（Cards）、操作按钮（Buttons）、攻略标题、标签徽章（Badges）** 中直接使用原生 Emoji（如 🍜, 🛥️, 🎮, 💰 等）裸排作为正式视觉图标。
* **原因**：Emoji 跨平台表现不可控（Windows 端显示为扁平卡通的 Segoe UI Emoji，风格与科技/游戏站极度割裂）；且 Emoji 无法通过 CSS 调整颜色与发光特效。

### 2. 图标选型分级规范（免署名标准）
根据业务场景分为两层结构，**100% 免费且必须【免署名（No Attribution Required）】**：

#### 层级 A：游戏核心特性 / 物品卡片（优先使用 CC0 专属矢量 SVG）
* **适用场景**：游戏特色卡片（如 Ramen Noir 拉面、Hover-boat 悬浮飞艇、黑市采购箱、夜总会鸡尾酒）。
* **【严禁】** 粗暴使用通用的办公线框图标硬套（**严禁用西餐刀叉代表拉面、严禁用大货轮代表赛博飞艇**）。
* **标准方案**：将高质量专属 SVG 文件保存在本地 `./assets/icons/`（如 `ramen.svg`, `hoverboat.svg`, `procurement.svg`, `cocktail.svg`）。
* **展示规范**：外层包裹带发光描边的暗黑道具槽：
  ```html
  <div class="w-12 h-12 rounded-xl bg-cyan-950/40 border border-cyan-500/30 p-2.5 mb-4 flex items-center justify-center shadow-lg shadow-cyan-950/50">
    <img src="assets/icons/ramen.svg" alt="Ramen Noir" class="w-full h-full object-contain" width="48" height="48" loading="lazy">
  </div>
  ```

#### 层级 B：常规 UI 辅助与交互按钮（使用 Remix Icon / SVG）
* **适用场景**：外链箭头、关闭、搜索放大镜、菜单折叠等通用 UI 部件。
* **协议要求**：Apache 2.0 / MIT 开源协议，无需页脚署名。
* **CDN 引入**：
  ```html
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/remixicon@4.2.0/fonts/remixicon.min.css">
  ```

---

## 🚀 二、 静态站点工程与 SEO 规范 (Engineering & SEO)

1. **Meta 与结构化数据**：
   * 所有 HTML 必须包含完整的 `title`, `description`, `canonical`, Open Graph (`og:*`), Twitter Card。
   * 必须包含 Schema.org JSON-LD 结构化数据（如 `FAQPage`, `VideoGame`, `WebSite`）。
2. **免服与极速加载**：
   * 本地 SVG 矢量图标必须添加 `width`, `height`, `alt` 属性，并添加 `loading="lazy"`。
   * 优先使用已编译的 CSS（如 `style.css`）。
3. **出海规范**：
   * 页面主语言遵循目标语系（默认 `lang="en"`）。
   * 严禁在面向海外用户的正式页面上展示未翻译中文。

---

## 🌐 三、 官方外链与 GitHub 组织规范 (Official Backlinks & Organization Standards)

1. **统一组织归属**：
   * 所有游戏攻略、伴侣工具、开源 Wiki 的公开 GitHub 仓库，**必须且只能归属在官方组织**：`https://github.com/open-game-wiki`。
   * 仓库命名规范：`open-game-slug-guides`（如 `open-game-wiki/nivalis-nights-guides`）。
2. **仓库标准化要求**：
   * 必须设置为 **Public**（公开），开启 Homepage 并指向对应独立站生产域名。
   * `README.md` 顶部必须包含指向独立站各核心功能页的动态 Shields 徽章与 Markdown 矩阵导航表。
   * 配置 MIT 开源协议以获得完整的仓库评分。
   * 与外部媒体长文（如 Medium 等）互相交织引用，构建高权重开源引流网络。
