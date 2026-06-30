# 复习知识库

基于 GitHub Pages 的静态复习资料站点，将课程复习材料从 Word/PDF 转换为在线可访问的 HTML 页面。

## 站点地址

- 首页入口: https://aeuicey.github.io/cailiao.github.io/
- 内容列表: https://aeuicey.github.io/cailiao.github.io/list.html
- 公考知识库（Test阶段）: https://aeuicey.github.io/cailiao.github.io/html/gksz/GK索引.html
- 关于页面: https://aeuicey.github.io/cailiao.github.io/html/about.html

## 技术栈

- Typora 导出 HTML（Pixyll 主题）作为内容页面基底
- GitHub Actions 自动部署（push to main → gh-pages）
- 原生 Canvas 动画（首页银色金属丝波动、关于页樱花飘落与波浪）
- GitHub REST API 客户端数据获取（关于页统计数据）

## 当前内容

### 大二

- 土木工程材料
- 哲学基础
- 经济学

### 大三

- 经济法 / 经济法补
- 钢混迅速上手复习资料（外部链接，由 @Alicedreve 提供 PDF 存储与预览）
- 毛概复习资料
- 习思想复习资料

### 公考资料（Test阶段）

- 公考知识库索引（GK索引）
- 热点夜话系列文章（3篇）

## 页面说明

| 页面 | 文件 | 说明 |
|------|------|------|
| 首页入口 | `index.html` | 项目介绍页，链接到内容列表、公考知识库、Alicetec 官网等 |
| 内容列表 | `list.html` | 主页，明日方舟风格深色主题 + 银色金属丝 Canvas 动画 |
| 关于 | `html/about.html` | 个人介绍，深色主题 + 樱花飘落 + 银色波浪动画 + GitHub 统计 |
| 复习资料 | `html/dasan/*.html` `html/daer/*.html` | 各科目复习材料，Typora 导出 HTML |
| 公考知识库 | `html/gksz/GK索引.html` | 公考资料索引页 + 热点夜话系列文章（Test阶段） |

## 项目结构

```
cailiao.github.io/
├── .github/workflows/deploy.yml   # GitHub Actions 部署工作流
├── html/
│   ├── about.html                 # 关于页面
│   ├── daer/                      # 大二复习资料
│   ├── dasan/                     # 大三复习资料
│   └── gksz/                      # 公考资料（GK索引 + 热点夜话）
├── MD/                            # 原始 Markdown 文件
├── index.html                     # 首页入口
├── list.html                      # 内容列表页
└── README.md
```

## 本地预览

```bash
git clone https://github.com/aeuicey/cailiao.github.io.git
cd cailiao.github.io
# 直接用浏览器打开 list.html 即可
```

## 部署

推送至 `main` 分支后，GitHub Actions 自动构建并部署到 `gh-pages` 分支，站点即时更新。

## 贡献者

- @aeuicey — 项目维护、内容整理、页面开发
- @Alicedreve — PDF 存储与预览支持
