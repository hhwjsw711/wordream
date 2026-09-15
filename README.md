---
AIGC:
  ContentProducer: '001191110102MAD55U9H0F10002'
  ContentPropagator: '001191110102MAD55U9H0F10002'
  Label: '1'
  ProduceID: '61c2da60-2760-4adf-9c5a-7e6113d6419c'
  PropagateID: '61c2da60-2760-4adf-9c5a-7e6113d6419c'
  ReservedCode1: '86771efc-75b8-4359-8134-6e6f8a924ac5'
  ReservedCode2: '86771efc-75b8-4359-8134-6e6f8a924ac5'
---

# Wordream — Landing Page

[Wordream](https://wordream.com) 的官网 landing page。Prompt-to-Video AI Creator for iPhone。

线上地址：**https://wordream.com**

## 项目说明

- 一比一复刻 [reelful.app](https://www.reelful.app/) 新版首页的视觉与动效（品牌替换为 Wordream）
- 技术栈：Astro 7 + Tailwind CSS v4 + GSAP 3.15（ScrollTrigger）+ Lenis 平滑滚动
- 9 个页面：首页、Compare 索引 + 4 个对比详情页（vs CapCut / Edits / Captions / video-editing MCPs）、Terms、Privacy、Contact
- 动效：Hero 入场时间线、滚动视差、区块 reveal、磁性按钮、showcase 轮播（点激活卡切静音、触摸滑动、视频预加载首帧）
- 滚动条：桌面隐藏原生滚动条仅显示自定义橙色滚动条，触屏显示原生橙色细条
- SEO：JSON-LD（SoftwareApplication + Article）、og:image、canonical、manifest
- 无障碍：reduced-motion 关怀、aria 同步、focus-visible

## 页面清单

| 路径 | 页面 |
|---|---|
| `/` | 首页（Hero / Why / How it works / Pricing / CTA） |
| `/compare` | 对比索引页 |
| `/compare/reelful-vs-capcut` | Wordream vs. CapCut |
| `/compare/reelful-vs-edits` | Wordream vs. Edits (by Instagram) |
| `/compare/reelful-vs-captions` | Wordream vs. Captions |
| `/compare/reelful-vs-mcp-editors` | Wordream vs. video-editing MCPs |
| `/terms` | Terms of Service |
| `/privacy` | Privacy Policy |
| `/contact` | Contact |

## Commands

| Command           | Action                                           |
| :---------------- | :----------------------------------------------- |
| `bun install`     | Installs dependencies                            |
| `bun dev`         | Starts local dev server at `localhost:4321`      |
| `bun build`       | Build your production site to `./dist/`          |
| `bun preview`     | Preview your build locally, before deploying     |
| `bun astro ...`   | Run CLI commands like `astro add`, `astro check` |

## 部署

- 托管：Vercel（push 即自动部署）
- DNS：Cloudflare（仅 DNS 模式，不套代理）
- CTA 占位链接 `https://apps.apple.com/app/wordream` 待 App 上架后替换为真实 App Store 链接

## TODO

- [ ] App 上架后替换 CTA 占位链接
- [ ] 接入 GA / Meta Pixel / Clarity（等账号）
- [ ] OneLink UTM 归因（等 OneLink 账号）

> AI生成