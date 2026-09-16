# 娱乐阅读订阅：小说＋漫画

用于官方版 LeechBlock NG 的**单一域名订阅**，范围仅小说、漫画阅读站点，不代表所有娱乐类别。

## 推荐订阅

**[entertainment-domains.txt — 3,375 个去重域名](https://raw.githubusercontent.com/yzy-lex/reading-blocklists/main/entertainment-domains.txt)**

一个规则组即可覆盖小说与漫画，并统一设置拦截时间。纯文本，每行一个域名。

## 官方版 LeechBlock 接入

1. 建立一个“娱乐阅读”规则组。
2. 在 Advanced Options → **Load list of sites from URL** 填入上面的原始文件直链。
3. 分别在各浏览器设置相同的时间和星期；订阅只同步域名，不同步时段、锁配置或独立正则字段。
4. 不在这个域名组附加关键词条件。内容关键词应另设组；否则域名拦截也可能被关键词条件限制。

远程列表是完整替换，不是追加本地列表。需要个人补充时另建组。初次使用先检查正常页面，保留可修改设置的窗口；不要随意扩大到综合平台根域名。

列表在浏览器启动或设置变更时加载，并非GitHub提交后实时推送。见[官方说明](https://www.proginosko.com/leechblock/faq/load-from-url/)。

## 兼容保留的分类列表

| 列表 | 域名条数 | 原始文件 |
|---|---:|---|
| 小说 | 1,258 | [novel-domains.txt](https://raw.githubusercontent.com/yzy-lex/reading-blocklists/main/novel-domains.txt) |
| 漫画 | 2,124 | [comic-domains.txt](https://raw.githubusercontent.com/yzy-lex/reading-blocklists/main/comic-domains.txt) |

两表有7个共同域名，合并后为3,375个。旧链接继续可用；如果使用合并订阅，无需再同时订阅这两个分类列表。

## 状态与局限

- 更新：2026-09-16。初版过度依赖GitHub许可证自动识别，排除了聚合源独有条目。本版核实该来源README中的AGPL-3.0声明后，补回865个小说、32个漫画域名；来源依据见[SOURCES.md](SOURCES.md)。
- 三个纯文本文件是可编辑的分发源形式。公开列表不含个人阅读观察条目、浏览器配置或访问日志。
- 这是**候选域名列表**，不是内容识别器。旧域名可能失效或转手，条目数不是准确率。
- 通过官方LeechBlock NG 1.7.3解析函数的离线兼容检查；尚未完成所有浏览器的加载/误伤验收。
- 本仓库不会执行结构识别代码，也不包含未通过验收的正文正则。
- 当前为人工审核发布，没有自动跟踪上游或定期更新的承诺。

## 许可

衍生列表与说明采用GNU AGPL v3，并保留上游版权和许可要求。完整文本见LICENSE及LICENSES。上游作者不为本项目筛选结果背书。未复制小说、漫画正文或上游可执行代码。
