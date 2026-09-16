# 来源与修改记录

初始发布及合并更新：2026-09-16。仅静态提取站点标识，去除www前缀、筛选、去重、排序；不执行上游代码。计数可重叠，不应相加。

| 来源 | 本次使用范围 | 上游许可 | 贡献的独立域名数 |
|---|---|---|---:|
| [XIU2/Yuedu](https://github.com/XIU2/Yuedu) | shuyuan中的文本书源地址 | GPL-3.0 | 19 |
| [freeok/so-novel](https://github.com/freeok/so-novel) | BOOK_SOURCES.md中的站点链接 | AGPL-3.0 | 25 |
| [manga-download/hakuneko](https://github.com/manga-download/hakuneko) | 带manga标签的适配器网址和默认配置 | Unlicense | 794 |
| [lncrawl/lightnovel-crawler](https://github.com/lncrawl/lightnovel-crawler) | sources/_index.json的supported项，按has_manga分类 | GPL-3.0 | 302 |
| [keiyoushi/extensions-source](https://github.com/keiyoushi/extensions-source) | src中的baseUrl及明确镜像声明 | Apache-2.0 | 1409 |
| [JimmXinu/FanFicFare](https://github.com/JimmXinu/FanFicFare) | fanficfare/adapters的getSiteDomain字面量；排除测试/综合论坛 | Apache-2.0 (adapter code) | 90 |
| [aoaostar/legado](https://github.com/aoaostar/legado) | 聚合书源的站点标识；按类型、名称和网址筛选 | README明确声明AGPL-3.0，见下文 | 919 |

## 上游归属

- XIU2/Yuedu：XIU2及该项目贡献者，GPL v3。
- so-novel：freeok及该项目贡献者，AGPL v3。
- HakuNeko：manga-download项目贡献者，Unlicense。
- Lightnovel Crawler：lncrawl项目贡献者，GPL v3。
- Keiyoushi：Javier Tomás（上游许可声明Copyright 2015）及项目贡献者，Apache 2.0。
- FanFicFare：项目作者及贡献者。上游LICENSE明确fanficfare/webservice目录采用Apache许可；calibre-plugin另用GPL v3，本项目未使用该插件代码。

- aoaostar/legado：aoaostar及聚合源原贡献者。main/release README均声明AGPL-3.0；保留原作者归属，不以本站名义重新声明为原创站点库。

## 聚合源许可核对更正

初版把GitHub API未识别许可证（null）当作排除依据，未进一步核对README。2026-09-16核实以下两份第一方文件，均有`license-AGPL--3.0`徽章：

- [main/README.md](https://github.com/aoaostar/legado/blob/main/README.md)
- [release/README.md](https://github.com/aoaostar/legado/blob/release/README.md)

GitHub许可证接口和根目录LICENSE路径仍未返回独立许可文件；本次采用维护者README的明确声明作为来源依据，不宣称GitHub自动识别已修复，也不宣称逐个原始贡献者的权利链已被独立审计。只分发经提取筛选的域名标识，不复制聚合包、规则代码、正文、主题或账号配置。

补回865个小说和32个漫画域名，旧分类直链保留；新增合并直链。个人观察项仍不纳入。

## 发布筛选

- 只采用上表来源提供的域名证据；同一个域名也可能在其他公共列表出现。
- 不因一次网络超时删除站点，也不将HTTP 200当作内容正确的证明。
- 元数据或上游结构可能错误，旧域名可能失效或转手。用户可提交误伤或漏网反馈。
- 本项目对上游数据作了提取和筛选，不是原项目原样发布，也不代表原项目官方推荐。

## 文件校验（当前版本）

- `novel-domains.txt`：SHA-256 `ced853a86b2111f9737a47924e67435142123ae40d5664ef95059f1bf523b8a0`
- `comic-domains.txt`：SHA-256 `ec9476b24c2287427285c0289d8d0fcd2b8108f1850a6375f33c38aeeac1249d`
- `entertainment-domains.txt`：SHA-256 `14585a580b6e49abc918d3c01749001974f9f0533d06ef546ccd8e0a8f01ca60`
