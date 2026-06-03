# 🌐 Global AI Tools Directory

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Deployed-brightgreen)](https://9420166.xyz)
[![SEO Ready](https://img.shields.io/badge/SEO-Ready-success)](https://developers.google.com/search)

> 一个精心整理的全球 AI 工具导航站，收录顶尖大语言模型、AI 绘图、视频生成、3D 工具、数字人、生产力工具及 AI 智能体平台。每日更新，多语言支持，为开发者和创作者提供快速发现优质 AI 资源的入口。

## ✨ 主要特性

- **7 大分类**：LLM & Chat、Image & Art、Video Motion、3D & Spatial、Human & Face、AI Tools、AI Agents
- **50+ 精选工具**：DeepSeek、ChatGPT、Gemini、Midjourney、Runway、Sora、Coze、Dify 等
- **多语言支持**：English、简体中文、Español、日本語（前端动态切换）
- **响应式设计**：完美适配桌面、平板、手机
- **SEO 优化**：独立页面 + 站点地图 + robots.txt
- **极速加载**：纯静态 HTML/CSS/JS，无第三方依赖（除 Font Awesome 和广告）

## 📁 项目结构
ai-tools-directory/
├── index.html # 首页（全部分类展示）
├── ai-chat.html # 🤖 大语言模型与 AI 对话
├── ai-image.html # 🎨 AI 绘图与视觉艺术
├── ai-video.html # 🎬 前沿 AI 视频生成
├── ai-3d.html # 🗿 AI 3D 建模与空间计算
├── ai-human.html # 🧑‍🚀 AI 数字人与换脸
├── ai-tools.html # ⚡ AI 生产力工具箱
├── ai-agents.html # 🤖 AI 智能体与无代码平台
├── sitemap.xml # 站点地图（供搜索引擎提交）
├── robots.txt # 爬虫协议文件
├── CNAME # 自定义域名（www.9420166.xyz）
└── README.md # 项目说明

text

## 🚀 快速部署

### 方式一：使用 GitHub Pages（推荐）

1. **Fork 本仓库** 或 **新建仓库** 并将所有文件上传
2. 进入仓库 `Settings` → `Pages`
3. 在 **Branch** 选择 `main`，文件夹选择 `/ (root)`
4. 保存后等待 1-2 分钟，网站即通过 `https://你的用户名.github.io/仓库名/` 访问
5. **绑定自定义域名**（可选）：在仓库根目录添加 `CNAME` 文件（内容为你的域名），并在 DNS 服务商处配置 A/CNAME 记录指向 GitHub Pages

### 方式二：本地运行

```bash
# 克隆仓库
git clone https://github.com/你的用户名/ai-tools-directory.git

# 进入目录
cd ai-tools-directory

# 使用任意 HTTP 服务器（例如 Python）
python3 -m http.server 8000
# 或使用 VS Code Live Server 插件
打开浏览器访问 http://localhost:8000

🔧 自定义与维护
添加新工具
每个分类页面（如 ai-chat.html）中的卡片网格采用统一结构：

html
<a href="工具官网链接" target="_blank" class="card">
  <div class="card-header">
    <i class="fa-solid fa-icon"></i>
    <h3>工具名称</h3>
  </div>
  <p class="lang-data" 
     data-en="English description"
     data-zh="中文描述"
     data-es="Descripción en español"
     data-ja="日本語の説明">
  </p>
</a>
只需复制上述代码块并修改 href、图标、名称和多语言描述即可。

更新多语言文案
所有多语言文本集中定义在页面底部的 <script> 中的 i18n 对象。修改对应键值对即可全局生效。

修改站点地图
sitemap.xml 中列出了所有重要页面。每次新增页面后，请同步添加对应的 <url> 条目，并更新 <lastmod> 日期。

🔍 SEO 配置
robots.txt：允许所有爬虫抓取，并指定了站点地图位置

sitemap.xml：包含首页及 7 个分类页，并添加了图片扩展信息，有助于图片搜索收录

独立页面：每个分类拥有独立 HTML 文件，URL 无锚点，利于搜索引擎索引

语义化标题：每个页面都有独立的 <title> 和 <meta description>

Canonical 标签：每个页面头部添加了 rel="canonical" 指向自己的 URL，避免重复内容

📌 部署后请记得在 Google Search Console 中提交 sitemap.xml，并在 Bing Webmaster Tools 中验证网站。

📡 广告与第三方资源
Google AdSense：已在页面中集成广告位（数据-ad-client 为 ca-pub-1624261597740761）

Font Awesome：通过 CDN 引入图标库（v6.4.0），用于美化界面

如需移除广告，请删除 <div class="ad-container"> 及其内部的 <ins> 标签和对应的 <script> 初始化代码。

🌟 贡献指南
欢迎提交 Issue 或 Pull Request 来添加新的 AI 工具、修复错别字或改善样式。

Fork 本仓库

创建你的特性分支：git checkout -b feature/NewTool

提交更改：git commit -m 'Add new AI tool: xxx'

推送到分支：git push origin feature/NewTool

提交 Pull Request

📄 许可证
本项目采用 MIT 许可证，你可以自由使用、修改和分发，但请保留原始版权声明。

📧 联系方式
网站：https://www.9420166.xyz

邮箱：ai@toolhub.com
