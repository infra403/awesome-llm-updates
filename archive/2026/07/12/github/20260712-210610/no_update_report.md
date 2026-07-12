# GitHub 项目巡检运行记录

- 时间：2026-07-12 21:06 北京时间
- 结果：本周期候选列表为空，未产生可写入固定 Feishu 文档的 P0/P1 仓库条目。
- 原因：预运行脚本返回 `NO_NEW_CANDIDATES`；同时 GitHub 多个 topic 查询因 HTTP 403 rate limit exceeded 失败。
- 写入动作：未追加 GITHUB_DOC_URL / TIME_DOC_URL / TOPIC_DOC_URL，避免写入空条目或低置信度内容。

## Fetch Failures

- topic:llm pushed:>=2026-07-12 stars:>20 sort=updated：HTTP Error 403: rate limit exceeded
- topic:llm pushed:>=2026-07-12 stars:>20 sort=stars：HTTP Error 403: rate limit exceeded
- topic:ai-agent pushed:>=2026-07-12 stars:>10 sort=updated：HTTP Error 403: rate limit exceeded
- topic:ai-agent pushed:>=2026-07-12 stars:>10 sort=stars：HTTP Error 403: rate limit exceeded
- topic:rag pushed:>=2026-07-12 stars:>10 sort=updated：HTTP Error 403: rate limit exceeded
- topic:rag pushed:>=2026-07-12 stars:>10 sort=stars：HTTP Error 403: rate limit exceeded
- topic:mcp pushed:>=2026-07-12 stars:>10 sort=updated：HTTP Error 403: rate limit exceeded
- topic:mcp pushed:>=2026-07-12 stars:>10 sort=stars：HTTP Error 403: rate limit exceeded
- large-language-model pushed:>=2026-07-12 stars:>20 sort=updated：HTTP Error 403: rate limit exceeded
- large-language-model pushed:>=2026-07-12 stars:>20 sort=stars：HTTP Error 403: rate limit exceeded
