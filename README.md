# Kickoff ⚽ — Web Mirror

> **此仓库仅托管 Kickoff App 官网与法律协议页面。**
>
> **完整源代码不在此处，禁止向本仓库提交任何源码。**

## 仓库职责

| 仓库 | 职责 | URL |
|---|---|---|
| **Gitee Football**（代码主仓） | 完整 iOS 源码 / 单元测试 / 文档 / 决策记录 / 自动化脚本 | <https://gitee.com/ai_project_shun/Football> |
| **GitHub kickoff**（本仓库） | **仅** 官网 + 法律协议（GitHub Pages 部署） | <https://github.com/flashbody/kickoff> |

## GitHub Pages 上线地址

- 官网首页：<https://flashbody.github.io/kickoff/>
- 隐私政策（Privacy Policy）：<https://flashbody.github.io/kickoff/privacy.html>
- 服务条款（Terms of Service）：<https://flashbody.github.io/kickoff/terms.html>
- 404 页面：<https://flashbody.github.io/kickoff/404.html>

## 目录说明

```
kickoff/                 # GitHub 仓库（仅托管 web/ 与协议）
├── web/                 # 官网 + 法律协议（多语种 HTML）
│   ├── index.html       # Landing 页
│   ├── privacy.html     # 隐私政策
│   ├── terms.html       # 服务条款
│   ├── 404.html
│   ├── robots.txt
│   └── sitemap.xml
├── LICENSE              # 专有许可证
└── README.md            # 本文件
```

## 部署流程

`web/` 目录通过 `gh-pages` orphan 分支独立部署，与 `main` 分支零污染。

代码主仓（Gitee）下执行：

```bash
bash scripts/pages_publish.sh
```

该脚本会把 `web/` 目录的内容强推到 GitHub `gh-pages` 分支（orphan 历史，不携带源码）。

## 严格禁止

- ❌ 严禁将 `Kickoff/`、`KickoffTests/`、`KickoffWidget/`、`KickoffWatch/` 等源码目录提交到本仓库
- ❌ 严禁将 `docs/`、`adr/`、`scripts/`、`project.yml` 等开发文件提交到本仓库
- ❌ 严禁将 API Key、签名证书、profile、`.entitlements` 等敏感文件提交到本仓库

## 法律声明

Kickoff 与 FIFA 无任何隶属关系。"World Cup"、"FIFA" 系 FIFA 注册商标。

Proprietary © 2026 Kickoff Studio. All rights reserved.
