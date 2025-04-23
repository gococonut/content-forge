# ContentForge - 智能内容创作引擎

ContentForge 是一个智能化的内容创作和管理系统，能够自动化生产多种形式的优质内容，包括播客、文章、笔记和社交媒体分享内容。通过 N8N 工作流引擎，系统可以灵活配置不同的内容生产流程，满足多样化的创作需求。

## 🌟 特性

- 🎙️ 播客制作
  - 文本转优质语音
  - 自动生成 Show Notes
  - 播客元数据管理

- 📝 文章创作
  - 智能文章生成
  - 多语言内容适配
  - SEO 优化建议

- 📒 知识管理
  - 笔记自动提取
  - 知识点归类
  - 标签智能推荐

- 🚀 社交传播
  - 多平台内容适配
  - 话题标签推荐
  - 发布时间优化

## 🏗️ 系统架构

### 后端服务

1. **N8N 工作流服务**
   - 可视化工作流编排
   - 多样化触发方式（Webhook、定时、手动）
   - 灵活的内容处理流程
   - 丰富的第三方集成

2. **TTS 服务**
   - 基于 MiniMax API
   - 自然流畅的语音合成
   - 支持长文本分段处理
   - 多音色选择

3. **GitHub Trending API**
   - 技术内容聚合
   - 热门项目分析
   - 技术趋势洞察

### 前端应用 (开发中)

- Next.js 构建的现代化 Web 界面
- 统一的内容管理中心
- 实时工作流监控
- 数据分析仪表板

## 🚀 快速开始

### 环境要求

- Docker & Docker Compose
- Node.js 18+
- Python 3.8+

### 配置环境变量

1. 创建环境配置：
\`\`\`bash
cp .env.example .env
\`\`\`

2. 配置必要的环境变量：
\`\`\`env
# N8N 配置
N8N_DOMAIN=your_n8n_domain
N8N_PORT=8000

# MiniMax API
MINIMAX_API_KEY=your_api_key
MINIMAX_GROUP_ID=your_group_id
\`\`\`

### 启动服务

1. 启动后端服务：
\`\`\`bash
docker-compose up -d
\`\`\`

2. 启动前端开发服务器（开发中）：
\`\`\`bash
cd frontend
npm install
npm run dev
\`\`\`

## 📁 项目结构

\`\`\`
.
├── docker-compose.yml    # Docker 服务编排配置
├── tts/                 # TTS 服务
│   ├── app/            # TTS 应用代码
│   └── Dockerfile      # TTS 服务构建文件
├── frontend/           # Next.js 前端应用 (开发中)
└── output/            # 生成的内容
    ├── audio/         # 音频文件
    ├── articles/      # 生成的文章
    ├── notes/         # 知识笔记
    └── social/        # 社交媒体内容
\`\`\`

## 🔄 工作流示例

1. **内容采集**
   - 网页内容抓取
   - 表单数据收集
   - API 数据集成
   - 批量内容导入

2. **智能处理**
   - 内容优化和结构化
   - 关键信息提取
   - 多语言处理
   - SEO 优化

3. **多形态转换**
   - 播客音频制作
   - 文章生成
   - 笔记提取
   - 社交文案创作

4. **智能分发**
   - 多平台发布
   - 定时发布
   - 数据追踪
   - 效果分析

## 🛠️ 开发计划

- [ ] Next.js 前端界面
- [ ] 内容模板系统
- [ ] AI 驱动的内容优化
- [ ] 多语言支持
- [ ] 数据分析系统
- [ ] API 文档
- [ ] 自动化测试
- [ ] 用户协作功能

## 📝 使用许可

[MIT](LICENSE)

## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request！

1. Fork 本仓库
2. 创建特性分支
3. 提交变更
4. 推送到分支
5. 创建 Pull Request

## 📮 联系方式

- 项目作者：[Your Name]
- 邮箱：[Your Email]
- 项目主页：[Project URL]