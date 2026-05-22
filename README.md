# CharaStudio

> A character and story-centric AIGC end-to-end creation tool — v1.0.0-beta

---

## What is CharaStudio

CharaStudio is a **character-driven** AIGC end-to-end creation software, dedicated to helping creators complete all stages — from character design, story creation, image generation, to comic production — on a single unified platform.

We believe the soul of every compelling story is a vivid character. CharaStudio deeply integrates AI capabilities into every stage of the creative workflow: AI-assisted brainstorming, AI-generated images, AI-driven conversations… freeing creators from tedious details so they can focus on the characters and stories that matter most.

### Vision

> **Empower everyone to effortlessly create their own character universe.**

Whether you're a novelist, game designer, comic creator, or a casual character chat enthusiast, CharaStudio aims to be the most handy creation tool in your hands.

---

## Core Modules

| Module | Description | Status |
|--------|-------------|--------|
| **Character** | Character card creation, character chat, image gallery management | **Beta** |
| **Story** | Complete workflow: outline → volumes → storylines → chapter scripts → chapter content | Planned |
| **Asset** | World cards, scene cards, item cards, effect cards; supports prompt steganography | Planned |
| **Comic** | Novel/script import → episodes → scenes → panels → image generation | Planned |
| **Drama** | — | Planned |

> **Beta Note**: v1.0.0-beta has opened character creation and character chat functions. Other modules are under development.

---

## Features in Beta

### Character Creation

#### Character Information Management

Complete character information editing capabilities covering every aspect of character design:

- **Basic Info** — Name, aliases, gender, age, role (protagonist / antagonist / supporting / background)
- **Tag System** — Preset and custom tags (personality traits, strengths & weaknesses, habits, build, hairstyle, skin tone, eye color, features, accessories, etc.), supporting quick filtering
- **Backstory** — Overview, world view / faction, family background
- **Personality** — Traits, strengths, weaknesses, habits, fears and desires
- **Physical Description** — Height & build, hair style & color, eyes, skin tone, clothing, distinctive features, accessories
- **Life Events** — Record key character events on a timeline
- **Character Relationships** — Add, edit, delete relationships with other characters
- **Meta Info** — Creator, version number, creator notes

#### AI-Assisted Character Creation

Built-in AI assistant (Agent) as your creative partner, available at any time in the character editor:

- **AI Filling Assistance** — Automatically enrich backstory, personality analysis, and relationship details based on existing information
- **Creative Dialogue** — Communicate with AI through natural language to get character design suggestions
- **Markdown Editor** — Write character descriptions in Markdown format with structured field parsing

#### Character Gallery

- **Upload Local Images** — Supports JPG, PNG, WebP, max 10MB per file
- **AI-Generated Character Images** — Two-step generation flow: ① LLM generates prompts → ② Image model renders
  - Selectable image types: portrait, four-view, expressions, poses, story moments
  - Selectable art styles and aspect ratios
  - Adjustable generation parameters (steps, CFG, etc.)
  - Save directly to character gallery after generation; first portrait is auto-set as cover
- **Gallery Management** — Batch delete, set cover, preview

---

### Character Chat

Enter the character detail page and start a real-time conversation with one click:

- **Streaming Responses** — Character replies stream in real time for a smooth, natural experience
- **Multi-Session Management** — Create new sessions, switch between sessions, delete sessions
- **Chat Export** — Export current conversation content
- **Character Profile Import / Export** — Easy backup and sharing of character cards

#### Chat Settings

- **Chat Mode** — Free switch between roleplay and narrative modes
- **Model Selection** — Specify which language model to use for generation
- **Generation Parameters** — Temperature, Max Tokens, TopP, minimum output length
- **Prompt Template Editor** — View, edit, reset system prompt templates for deep customization of character behavior

---

## System Features

### Model Management

CharaStudio supports flexible configuration of multiple AI models, covering the entire creation workflow:

- **Language Model (LLM)** — Supports OpenAI-compatible API; can connect to local or cloud-based language model services
- **Image Generation Model** — Supports configuration for mainstream text-to-image models
- **ComfyUI Model** — Supports official, custom, and local ComfyUI workflow models

All models can be managed and toggled on/off centrally in settings.

### User Management

- **Account System** — Register, login, personal information management
- **Data Export** — Export and back up user data

### System Settings

- **Language Switch** — Simplified Chinese, English, Japanese; real-time switching without restart
- **Style Preferences** — Customizable interface styling
- **Version Updates** — Automatic update detection and notifications

---

## Technical Architecture

CharaStudio is built on a modern tech stack, balancing performance and scalability:

| Layer | Technology |
|-------|------------|
| **Desktop Framework** | Wails (Go + Web Frontend) |
| **Backend** | Go |
| **Frontend** | React + TypeScript |
| **Browser Automation** | Playwright |
| **Database** | SQLite |

### Design Principles

- **Modular Functional Services** — Each feature module is independent and pluggable, facilitating extension and maintenance
- **Multi-Agent Architecture** — Collaborative mechanism based on MasterAgent + SubAgent; complex tasks are automatically decomposed and executed
- **Asynchronous Task Execution** — Background tasks are monitored in real time with transparent progress visibility
- **Extensible Agent Tool System** — Built-in Tool / MCP / Skill multi-layer tool system; AI capabilities are invoked on demand

---

## Roadmap

After the Beta release, CharaStudio will continue iterating, gradually opening the following modules:

- **Story Creation Module** — Complete pipeline: outline → volumes → storylines → chapter scripts → chapter content
- **Asset Management System** — World cards, scene cards, item cards, effect cards; supports prompt steganography
- **Comic Production Module** — One-stop flow from script to panel layouts to image generation
- **More AI Capabilities** — Scene generation, conversational illustration auto-matching, intelligent recommendations, etc.

We welcome all creators to try the Beta version and provide feedback — together we will shape the future of CharaStudio.

---

## Quick Start

1. Download and install CharaStudio v1.0.0-beta
2. In **Settings → Model Management**, configure the LLM (language model) and image generation model
3. Go to the **Character** module and start creating your first character
4. Upload or AI-generate a portrait image for your character
5. Enter the character detail page and click **Start Chat** to talk with the character

For detailed usage instructions, please refer to the main project documentation.

---

> CharaStudio is under active development — features are continuously updated. If you encounter any issues or have suggestions, feel free to share your feedback: charastudio@163.com.

---

# CharaStudio 查拉工作室

> 一款以角色和故事为中心的 AIGC 全流程创作工具 — v1.0.0-beta

---

## 什么是 CharaStudio

CharaStudio（查拉工作室）是一款专注于**角色驱动**的 AIGC 全流程创作软件，致力于让创作者在一个统一的平台上完成从角色设计、故事创作到图像生成、漫画制作的全部环节。

我们相信，每一个精彩故事的灵魂都是鲜活的角色。CharaStudio 将 AI 能力深度融入创作流程的每个阶段：AI 辅助构思、AI 生成图像、AI 驱动对话……让创作者从繁琐的细节中解放出来，专注于表达最核心的角色与故事。

### 愿景

> **让每个人都能轻松创作属于自己的角色宇宙。**

无论是小说作者、游戏策划、漫画创作者，还是纯粹的角色聊天爱好者，CharaStudio 都希望成为你手中最顺手的创作工具。

---

## 核心模块

| 模块 | 说明 | 状态 |
|------|------|------|
| **角色 (Character)** | 角色卡制作、角色聊天、角色图库管理 | **Beta** |
| **故事 (Story)** | 大纲→分卷→故事线→章节脚本→章节内容的完整创作流程 | 规划中 |
| **资产 (Asset)** | 世界卡、场景卡、物品卡、特效卡等，支持 prompt 隐写 | 规划中 |
| **漫画 (Comic)** | 小说/剧本导入 → 分集 → 分场 → 分镜 → 图像生成 | 规划中 |
| **短剧 (Drama)** | — | 规划中 |

> **Beta 版本说明**：v1.0.0-beta 已开放角色制作与角色聊天功能，其他模块正在开发中。

---

## Beta 版本已实现功能

### 角色制作

#### 角色信息管理

提供完整的角色信息编辑能力，涵盖角色设定的方方面面：

- **基础信息** — 角色名称、别名、性别、年龄、定位（主角 / 反派 / 配角 / 路人）
- **标签系统** — 预设及自定义标签（性格特点、优缺点、习惯、体型、发型、肤色、瞳色、特征、配饰等），支持快速筛选
- **背景故事** — 概述、世界观 / 势力、家庭背景
- **性格设定** — 性格特点、优点、缺点、习惯、恐惧与欲望
- **外貌描述** — 身高体型、发型发色、眼睛、肤色、服装、显著特征、配饰
- **人生历程** — 按时间线记录角色关键事件
- **角色关系** — 添加、编辑、删除与其他角色的关系
- **元信息** — 创建者、版本号、创作者备注

#### AI 辅助角色创作

内置 AI 助手（Agent）作为创作伙伴，可在角色编辑界面随时呼出：

- **AI 协助填充** — 根据已有信息自动补充背景故事、性格分析、关系完善等
- **创作对话** — 通过自然语言与 AI 交流，获得角色设定建议
- **Markdown 编辑器** — 支持 Markdown 格式编写角色描述，并可解析为结构化字段

#### 角色图库

- **上传本地图片** — 支持 JPG、PNG、WebP，单文件最大 10MB
- **AI 生成角色图** — 两步式生成流程：① LLM 生成提示词 → ② 生图模型出图
  - 可选图片类型：肖像、四视图、表情、动作、故事节点
  - 可选艺术风格及宽高比
  - 可调节步数、CFG 等生图参数
  - 生成后可直接保存至角色图库，并自动设为首张肖像图
- **图库管理** — 批量删除、设为封面、预览

---

### 角色聊天

进入角色详情页后，可一键开启与该角色的实时对话：

- **流式回复** — 角色回复实时流式输出，体验流畅自然
- **多会话管理** — 新建会话、切换会话、删除会话
- **对话导出** — 支持将当前对话内容导出
- **角色设定导入 / 导出** — 方便角色卡片的备份与分享

#### 聊天设置

- **对话模式** — 角色扮演 / 故事叙事 两种模式自由切换
- **模型选择** — 可指定用于生成的语言模型
- **生成参数** — Temperature、Max Tokens、TopP、最小输出字数
- **提示词模板编辑器** — 可查看、编辑、重置系统提示词模板，深度定制角色行为

---

## 系统功能

### 模型管理

CharaStudio 支持灵活配置多种 AI 模型，覆盖创作全流程：

- **语言模型 (LLM)** — 支持 OpenAI 兼容接口，可连接本地或云端语言模型服务
- **生图模型** — 支持主流文生图模型的接入配置
- **ComfyUI 模型** — 支持官方、自定义及本地 ComfyUI 工作流模型

所有模型均可在设置中统一管理、开闭切换。

### 用户管理

- **账号系统** — 注册、登录、个人信息管理
- **数据导出** — 支持用户数据的导出备份

### 系统设置

- **语言切换** — 中文（简体）、English、日本語，实时切换无需重启
- **样式偏好** — 界面样式自定义
- **版本更新** — 自动检测与版本更新提示

---

## 技术架构

CharaStudio 基于现代化的技术栈构建，兼顾性能与可扩展性：

| 层级 | 技术 |
|------|------|
| **桌面框架** | Wails（Go + Web 前端） |
| **后端** | Go |
| **前端** | React + TypeScript |
| **浏览器自动化** | Playwright |
| **数据库** | SQLite |

### 设计理念

- **模块化功能服务** — 各功能模块独立可插拔，便于扩展和维护
- **多代理架构** — 基于 MasterAgent + SubAgent 的协同机制，复杂任务自动分解执行
- **异步任务执行** — 后台任务实时监控，进度透明可见
- **可扩展 Agent 工具** — 内置 Tool / MCP / Skill 多层工具体系，AI 能力按需调用

---

## 后续规划

Beta 版本之后，CharaStudio 将持续迭代，逐步开放以下模块：

- **故事创作模块** — 大纲 → 分卷 → 故事线 → 章节脚本 → 章节内容的完整链路
- **资产管理系统** — 世界卡、场景卡、物品卡、特效卡，支持 prompt 隐写
- **漫画制作模块** — 从剧本到分镜再到图像生成的一站式流程
- **更多 AI 能力** — 场景生成、对话插图自动匹配、智能推荐等

欢迎所有创作者体验 Beta 版本并提供反馈，一起塑造 CharaStudio 的未来。

---

## 快速开始

1. 下载并安装 CharaStudio v1.0.0-beta
2. 在 **设置 → 模型管理** 中配置 LLM（语言模型）和生图模型
3. 进入 **角色** 模块，开始创建你的第一个角色
4. 为角色上传或 AI 生成一张肖像图
5. 进入角色详情页，点击 **开始聊天** 与角色对话

详细使用说明请参考主项目文档。

---

> CharaStudio 正在积极开发中，功能持续更新。如遇问题或有任何建议，欢迎反馈：charastudio@163.com。
