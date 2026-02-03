# Mizuki 业务展示平台：硅步工作室 2024 年 1 月 1 日版

# 🌸 硅步工作室 - 基于 Mizuki 二次开发的业务展示平台

本项目是**硅步工作室**基于 [Mizuki](https://github.com/matsuzaka-yuki/mizuki) 静态博客模板二次开发的业务展示与文档平台，保留原模板核心技术架构与功能特性，适配工作室「技术副业全链路服务」的业务场景，遵循原项目 Apache 2.0 开源协议。

硅步工作室理念：不积跬步，无以至千里  

2020年创立 | 轻资产运营 | 合规备案 | 「学习-沉淀-变现」全链路服务

[**🖥️ 硅步工作室演示地址**](https://guibu3.cn/) 

🌏 **文档语言:**

[](./README.md)**[简体中文](./README.md)**[](./README.md) /

基于 Mizuki 模板的高效架构，快速搭建符合工作室需求的业务展示平台，包含业务矩阵、案例展示、服务流程、价格体系等核心模块。

[📚 查看硅步工作室完整业务文档] ([guibu3.cn](https://guibu3.cn/)) →

<table>

<tr>

<td><img alt="业务展示页" src="docs/image/1.webp"></td>

<td><img alt="案例详情页" src="docs/image/2.webp"></td>

<td><img alt="服务流程页" src="docs/image/3.webp"></td>

</tr>

<tr>

<td><img alt="价格体系页" src="docs/image/4.webp"></td>

<td><img alt="关于我们页" src="docs/image/5.webp"></td>

<td><img alt="联系合作页" src="docs/image/6.webp"></td>

</tr>

</table>

### 🔧 硅步工作室二次开发改造

- **业务模块整合**：新增业务矩阵、案例展示、价格体系、合作流程等核心页面

- **品牌视觉适配**：全局替换 Logo、配色、字体，符合工作室品牌规范

- **功能场景定制**：关闭非必要功能（如动漫追踪），强化文档展示、业务查询能力

- **部署流程优化**：适配工作室官网域名，新增国内服务器部署配置

- **联系方式集成**：页面全局嵌入电话、邮箱、地址等商务对接入口

### 📐 原模板核心特性（完整保留）

- **组件配置重构**：模块化配置体系，支持动态组件管理与排序

- **布局系统优化**：左右侧边栏切换、智能目录定位、响应式布局适配

- **配置格式标准化**：TypeScript 类型安全保障，支持自定义组件扩展

- **代码性能优化**：精简冗余依赖、优化组件加载逻辑，提升页面渲染速度

---

## ✨ 核心功能（业务适配版）

### 🎨 设计与交互

- [x] 基于 Astro + Tailwind CSS 构建，保留原模板平滑动画与页面过渡

- [x] 明暗主题切换（支持系统偏好检测），适配工作室品牌色

- [x] 动态轮播横幅（展示工作室核心业务与理念）

- [x] 全响应式设计，适配 PC/移动端商务展示场景

- [x] 统一使用工作室指定字体体系，提升品牌辨识度

### 🔍 内容与搜索

- [x] 基于 Pagefind 的高级搜索（支持业务关键词、案例名称检索）

- [x] 增强 Markdown 功能，适配业务文档、案例说明书写规范

- [x] 自动生成文档目录 + 滚动定位，便于快速浏览长文档

- [x] 业务分类/标签体系（按毕设服务、文书服务、运营服务等分类）

- [x] 阅读时长估算，优化用户浏览体验

### 📱 特色业务页面

- [x] **业务矩阵页** - 展示五大核心业务详细介绍与优势

- [x] **成功案例页** - 分类展示国内/海外项目案例与成果数据

- [x] **价格体系页** - 清晰呈现各业务收费标准与服务套餐

- [x] **合作流程页** - 可视化展示需求沟通至售后维护全流程

- [x] **关于我们页** - 工作室简介、理念、联系方式完整呈现

### 🛠 技术特性

- [x] 增强代码块展示（适配技术文档、项目架构说明场景）

- [x] 图片优化 + PhotoSwipe 画廊（高清展示案例截图、业务场景图）

- [x] SEO 优化（适配国内搜索引擎，提升工作室业务曝光）

- [x] 评论系统集成（支持客户咨询、合作留言互动）

- [x] 性能优化（懒加载、缓存机制，保障国内访问速度）

## 🚀 快速部署指南

### 📦 安装部署

1. **克隆仓库（硅步工作室版）**

    ```Bash
    
    git clone https://github.com/guibu-studio/mizuki-business.git
    cd mizuki-business
    ```

2. **安装依赖**

    ```Bash
    
    # 安装 pnpm（未安装时）
    npm install -g pnpm
    
    # 安装项目依赖
    pnpm install
    ```

3. **配置工作室站点**

    - 编辑 `src/config.ts`：修改站点标题、副标题、品牌色等基础信息

    - 编辑 `src/content/business/`：更新业务介绍、案例数据、价格信息

    - 替换 `public/` 下的 `guibu-logo.png` 为工作室实际 Logo

4. **启动开发服务器**

    ```Bash
    
    pnpm dev
    ```

    本地预览地址：`http://localhost:4321`

### 🚀 部署方案

支持多种部署方式，优先适配国内访问场景：

- **国内服务器**：使用 `scripts/deploy-cn.sh` 脚本一键部署至工作室服务器

- **Vercel/Netlify**：关联 GitHub 仓库，自动部署

- **GitHub Pages**：使用内置 GitHub Actions 工作流部署

- **环境变量配置**（可选）：

    ```Bash
    
    # Umami 统计 API Key（如需统计访问数据）
    UMAMI_API_KEY=your_umami_api_key
    # bcrypt 加密盐值（默认12）
    BCRYPT_SALT_ROUNDS=12
    ```

⚠️ 请勿将 `.env` 文件提交至 Git，生产环境建议通过部署平台配置环境变量。

## 📝 业务文档前置模板

```YAML

---
title: 业务文档标题（必填）
published: 2024-01-01（发布时间，必填）
description: 文档简介（SEO/预览用）
image: ./cover.jpg（封面图，相对路径）
tags: [业务类型, 关键词]（如：毕设服务、Flask、跨境电商）
category: 业务分类（如：核心业务、成功案例、价格体系）
draft: false（草稿状态：true-仅内网可见，false-公开）
pinned: false（是否置顶：true-首页展示，false-默认）
guibu:
  author: 负责人（可选）
  updateTime: 2024-01-02（更新时间，可选）
---
```

## 🧩 Markdown 书写规范

- **提示框**：统一使用 `> [!NOTE]`（业务说明）/ `> [!WARN]`（注意事项）/ `> [!TIP]`（合作提示）

- **代码块**：技术相关文档需添加语言标识，示例：

    ```Python
    
    # 毕设服务核心技术示例（Flask）
    from flask import Flask
    app = Flask(__name__)
    ```

- **图片引用**：案例截图、业务场景图统一存放至 `src/assets/business/`，确保加载速度

- **链接格式**：外部链接（如官网）需添加 `target="_blank"`，内部业务链接使用相对路径

## ⚡ 常用命令

|Command|Action|
|---|---|
|`pnpm install`|安装依赖|
|`pnpm dev`|启动本地开发服务器（[localhost:4321](http://localhost:4321)）|
|`pnpm build`|编译生产版本至 ./dist/|
|`pnpm preview`|本地预览生产版本|
|`pnpm format`|格式化代码|
|`pnpm new-post <filename>`|创建新业务文档/案例页面|
|`pnpm deploy:cn`|部署至国内服务器（硅步工作室专属脚本）|
## 🎯 配置指南

### 🔧 基础配置

编辑 `src/config.ts` 定制工作室站点信息：

```TypeScript

export const siteConfig: SiteConfig = {
  title: "硅步工作室 - 技术副业全链路服务平台",
  subtitle: "不积跬步，无以至千里",
  lang: "zh-CN",
  themeColor: {
    hue: 180, // 工作室品牌色 Hue 值
    fixed: true, // 固定品牌色，隐藏主题切换器
  },
  banner: {
    enable: true,
    src: ["assets/banner/business1.webp", "assets/banner/business2.webp"], // 业务相关横幅图
    carousel: {
      enable: true,
      interval: 3, // 轮播间隔（秒）
    },
  },
};
```

### 📝 业务内容管理

- **新增业务文档**：运行 `pnpm new-post 文档名称`，按前置模板填写内容

- **编辑案例数据**：修改 `src/content/business/cases/` 下的 Markdown 文件

- **更新价格体系**：编辑 `src/content/business/pricing.md`

- **添加图片资源**：案例截图、业务图存放至 `src/assets/business/`

## ✏️ 贡献说明

本项目为硅步工作室内部业务展示平台，暂不开放外部贡献。如需内部优化迭代，遵循以下流程：

1. 从 `main` 分支创建功能分支（`git checkout -b feature/业务优化`）

2. 提交修改（`git commit -m '[guibu] 优化业务展示页面'`）

3. 推送分支（`git push origin feature/业务优化`）

4. 提交内部 Pull Request 审核

## 📄 协议说明

- 本项目基于 [Mizuki](https://github.com/matsuzaka-yuki/mizuki) 开发，遵循原项目 **Apache License 2.0** 开源协议

- 原模板基于 [Fuwari](https://github.com/saicaca/fuwari)（MIT License），相关版权信息已保留在 LICENSE.MIT 文件中

- 硅步工作室二次开发部分的代码同样遵循 Apache License 2.0 协议，仅限授权场景使用

## 🙏 致谢

- 原模板：[Mizuki](https://github.com/matsuzaka-yuki/mizuki) by matsuzaka-yuki - 提供高效稳定的技术架构基础

- 技术依赖：Astro、Tailwind CSS、Swup、Pagefind 等开源项目

- 硅步工作室团队：参与本项目二次开发与业务适配的所有成员

## 🍀 关于硅步工作室

专注技术副业领域，构建「学习-沉淀-变现」全链路业务体系，核心业务涵盖计算机毕设服务、专业文书撰写、自媒体运营、海外项目代工、跨境电商服务，累计服务客户500+，交付项目成功率98%+。


---

⭐ 若本项目对您的合作决策有帮助，欢迎在 GitHub 点亮 Star！商务合作请通过官网或邮箱联系我们～
