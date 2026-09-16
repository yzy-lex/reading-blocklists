# Reading Blocklists for LeechBlock NG

用于官方版 LeechBlock NG 的小说、漫画域名候选列表。**不是内容识别器，不保证无误伤或域名仍然有效。**

| 列表 | 域名条数 | 订阅直链 |
|---|---:|---|
| 小说 | 393 | [novel-domains.txt](https://raw.githubusercontent.com/yzy-lex/reading-blocklists/main/novel-domains.txt) |
| 漫画 | 2,092 | [comic-domains.txt](https://raw.githubusercontent.com/yzy-lex/reading-blocklists/main/comic-domains.txt) |

## 使用

1. 在各浏览器的 LeechBlock 中分别建立小说和漫画规则组。
2. 在 Advanced Options → **Load list of sites from URL** 填入对应直链。
3. 单独设置拦截时段、星期、隐私模式和锁配置；这些不会随域名订阅同步。
4. 域名组不要附加关键词条件。初次使用先检查正常页面，保留可修改设置的窗口。

本列表是完整替换列表，不是增量补丁。远程加载会替换该组的网站列表；如需个人补充，可独立建组。默认按明确列出的主机范围使用，不随意扩大到综合平台根域名。

官方说明：列表在浏览器启动或设置变更时加载，并非GitHub提交后实时推送。见[LeechBlock文档](https://www.proginosko.com/leechblock/faq/load-from-url/)。

## 范围与局限

- 初始发布：2026-09-16。这两个纯文本文件是可直接编辑的分发源形式，每行一个域名。
- 从公开阅读器/爬虫的站点声明提取，仅选用本轮已核对许可的来源。未纳入许可未确认的聚合源独有条目或私人补充记录。
- 没有复制小说、漫画内容、上游可执行代码、浏览器配置或访问日志。来源、修改方式、许可证见[SOURCES.md](SOURCES.md)。
- 上游声明不保证网站当前可用、未转手或符合用户希望拦截的范围；域名数量不是有效覆盖率。
- 已经通过官方LeechBlock NG 1.7.3解析函数的离线格式兼容检查；尚未完成各浏览器远程加载和逐站误伤验收。
- 正文关键词正则和结构识别代码不包含在此订阅中，也不会通过本仓库自动执行。
- 当前为静态人工审核发布，没有承诺自动跟踪上游或无人审核自动更新。

## 许可

本仓库分发的衍生列表与说明采用GNU AGPL v3；保留各上游的版权和许可证要求。完整AGPL文本见LICENSE，GPL/Apache/Unlicense文本见LICENSES。上游作者不为本项目筛选结果背书。
