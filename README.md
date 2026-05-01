# 🚀 AI效率指南 - SEO静态网站

## 项目概述

这是一个为SEO文章工厂准备的静态展示网站，用于发布AI工具测评、对比评测和写作工具推荐等文章。

### 技术栈
- **纯HTML5 + CSS3** — 无依赖，加载极快
- **响应式设计** — 适配桌面/平板/手机
- **SEO优化** — Schema.org结构化数据、Open Graph、Meta标签
- **Vercel一键部署** — 零配置即可上线

### 文件结构
```
seo-site/
├── index.html              # 首页（文章列表）
├── pages/
│   ├── article1.html       # 10个AI工具测评
│   ├── article2.html       # ChatGPT vs Claude vs Gemini
│   └── article3.html       # 7款AI写作神器
├── css/
│   └── style.css           # 全局样式
├── js/                     # 预留JS目录
├── images/
│   └── favicon.svg         # 网站图标
├── vercel.json             # Vercel部署配置
├── sitemap.xml             # 搜索引擎站点地图
├── robots.txt              # 爬虫规则
└── README.md               # 本文件
```

---

## 🎨 设计特点

1. **现代简约风格** — 紫色主题，专业感强
2. **粘性导航栏** — 毛玻璃效果，滚动不丢失
3. **卡片式布局** — 首页展示所有文章
4. **阅读体验优化** — 正文页面最大宽度780px，行高1.7
5. **SEO友好** — 每个页面独立的 title/description/keywords
6. **结构化数据** — Article JSON-LD 标记
7. **响应式设计** — 移动端自适应

---

## 🛠️ 部署方式

### 方案一：Vercel（推荐 ⭐）

**最简单的一键部署：**

1. 将 `seo-site/` 文件夹推送到 GitHub 仓库
2. 登录 [vercel.com](https://vercel.com)
3. 点击 "Add New Project" → 导入 GitHub 仓库
4. Framework Preset 选择 "Other"
5. Root Directory 填写 `seo-site`
6. 点击 Deploy！

**自定义域名（可选）：**
- Settings → Domains → 添加你的域名
- 配置 DNS CNAME/ANAME 记录

**替换域名：**
找到代码中所有的 `your-domain.vercel.app` 替换为你的实际域名。

### 方案二：GitHub Pages

1. 创建 GitHub 仓库（如 `yourname/seo-article-site`）
2. 上传 `seo-site/` 下的所有文件到仓库根目录
3. Settings → Pages → Source 选择 main branch
4. Site 路径选 `/ (root)`
5. 访问 `https://yourname.github.io/seo-article-site/`

**缺点：** 无法使用自定义 SSL 证书的子域名，URL 较长。

### 方案三：Cloudflare Pages

与 Vercel 类似，免费额度充足，CDN 速度快。

---

## 📝 后续操作

### 添加新文章时：

1. 在 `pages/` 下新建 `articleX.html`
2. 复制现有文章页面的 `<head>` 结构
3. 更新 title、description、canonical URL
4. 更新首页 `index.html` 的文章卡片
5. 更新 `sitemap.xml` 添加新URL
6. 重新部署

### 修改CSS：

直接编辑 `css/style.css`，所有页面即时生效。

---

## 📊 SEO Checklist

- [x] 每页独立 Title / Meta Description / Keywords
- [x] Canonical URL
- [x] Open Graph 标签
- [x] Schema.org Article 结构化数据
- [x] sitemap.xml
- [x] robots.txt
- [x] H1/H2/H3 标题层级正确
- [x] 响应式设计
- [x] 语义化 HTML5 标签
- [ ] 提交 Google Search Console（上线后）
- [ ] 提交 Bing Webmaster Tools（上线后）
- [ ] 设置 Brave Search 验证（上线后）

---

*创建于 2026-05-01 | AI效率指南编辑部*
