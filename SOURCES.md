# 来源与修改记录

初始发布：2026-09-16。仅静态提取站点标识，去除www前缀、筛选、去重、排序；不执行上游代码。计数可重叠，不应相加。

| 来源 | 本次使用范围 | 上游许可 | 贡献的独立域名数 |
|---|---|---|---:|
| [XIU2/Yuedu](https://github.com/XIU2/Yuedu) | shuyuan中的文本书源地址 | GPL-3.0 | 19 |
| [freeok/so-novel](https://github.com/freeok/so-novel) | BOOK_SOURCES.md中的站点链接 | AGPL-3.0 | 25 |
| [manga-download/hakuneko](https://github.com/manga-download/hakuneko) | 带manga标签的适配器网址和默认配置 | Unlicense | 794 |
| [lncrawl/lightnovel-crawler](https://github.com/lncrawl/lightnovel-crawler) | sources/_index.json的supported项，按has_manga分类 | GPL-3.0 | 302 |
| [keiyoushi/extensions-source](https://github.com/keiyoushi/extensions-source) | src中的baseUrl及明确镜像声明 | Apache-2.0 | 1409 |
| [JimmXinu/FanFicFare](https://github.com/JimmXinu/FanFicFare) | fanficfare/adapters的getSiteDomain字面量；排除测试/综合论坛 | Apache-2.0 (adapter code) | 90 |

## 上游归属

- XIU2/Yuedu：XIU2及该项目贡献者，GPL v3。
- so-novel：freeok及该项目贡献者，AGPL v3。
- HakuNeko：manga-download项目贡献者，Unlicense。
- Lightnovel Crawler：lncrawl项目贡献者，GPL v3。
- Keiyoushi：Javier Tomás（上游许可声明Copyright 2015）及项目贡献者，Apache 2.0。
- FanFicFare：项目作者及贡献者。上游LICENSE明确fanficfare/webservice目录采用Apache许可；calibre-plugin另用GPL v3，本项目未使用该插件代码。

## 发布筛选

- 只采用上表来源提供的域名证据；同一个域名也可能在其他公共列表出现。
- 不因一次网络超时删除站点，也不将HTTP 200当作内容正确的证明。
- 元数据或上游结构可能错误，旧域名可能失效或转手。用户可提交误伤或漏网反馈。
- 本项目对上游数据作了提取和筛选，不是原项目原样发布，也不代表原项目官方推荐。

## 文件校验（初始版本）

- `novel-domains.txt`：SHA-256 `6f93c3a73a8ee1bf7e3ae5a6231d045f7be2b4f6cd6184ff015f148b8e518b54`
- `comic-domains.txt`：SHA-256 `2281ceea12848ca1aedf8421560861b594464ca41cfa3d785ba6004e36ace7d0`
