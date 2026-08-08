## Hey, I'm Yufeng He 👋

AI Agents & LLM Systems Engineer | Formerly @ [Moonshot AI](https://www.moonshot.ai/) (Kimi) | MS CS @ HKU | Champion, Shanghai Global AI Contest | 3x ACM-ICPC Silver Medalist | Former Intern @ Baidu, Maimai, Kuaishou

- 370+ merged upstream PRs, with fixes in vLLM (9 merged), Mooncake (35 merged), Qwen Code (53 merged), Microsoft Agent Framework (26 merged), AstrBot (30 merged), Google ADK (10 merged), Inspect AI (22 merged), Hugging Face Transformers (1 merged), Kimi Code (1 merged), Vibe-Trading (8 merged), and PyTorch (8 merged).
- Selected public projects led by CoreCoder, FindJobs-Agent, RepoWiki, and ContractGuard.

### Projects

| Area | Project | Stars | Notes |
|------|---------|:-----:|-------|
| Coding agents / evals | [CoreCoder](https://github.com/he-yufeng/CoreCoder) | 1.6k+ | 512K lines of Claude Code → 1,400 lines of Python. Every key architectural pattern, runnable. Any LLM. 7 architecture deep-dive articles. |
| Applied agents | [FindJobs-Agent](https://github.com/he-yufeng/FindJobs-Agent) | 200+ | LLM-powered job toolkit: skill gap analysis, mock interviews, resume optimization, and job structuring. |
| Codebase maps | [RepoWiki](https://github.com/he-yufeng/RepoWiki) | 200+ | Open-source DeepWiki alternative: CLI/browser wiki generation, PageRank file ranking, Mermaid diagrams, and reading guides. |
| Applied agents | [ContractGuard](https://github.com/he-yufeng/ContractGuard) | 100+ | AI agent that reviews contracts for red flags before you sign: unfair terms, missing protections, and plain-English explanations. |
| Codebase maps | [GitSense](https://github.com/he-yufeng/GitSense) | 50+ | AI-powered contribution finder and repo radar: find matching issues, then check PR merge signals before spending a weekend. |
| Code understanding | [CodeABC](https://github.com/he-yufeng/CodeABC) | new | AI code reader for non-programmers: plain-language file guides, hover annotations, a terminology dictionary, Q&A, and natural-language edits. |
| Coding agents / evals | [AgentProbe](https://github.com/he-yufeng/AgentProbe) | new | Pytest plugin for regression-testing AI agents: snapshot baselines, semantic comparison, and mock LLMs. |
| Coding agents / evals | [AnyCoder](https://github.com/he-yufeng/AnyCoder) | new | AI coding agent CLI supporting 100+ LLMs via litellm, with dangerous command blocking, parallel tools, and session persistence. |
| Coding agents / evals | [CodeJoust](https://github.com/he-yufeng/CodeJoust) | new | CLI arena for AI coding agents: isolated `git worktree` runs, test/cost/diff/time scoring, and `pip install codejoust`. |
| Coding agents / evals | [LiteBench](https://github.com/he-yufeng/LiteBench) | new | Pip-installable LLM/agent benchmark CLI + web dashboard, with agent mode, custom YAML, LLM-as-judge, and 100+ litellm models. |
| Agent tooling | [RuleForge](https://github.com/he-yufeng/RuleForge) | new | Auto-generate AI assistant rules (CLAUDE.md, .cursorrules, copilot-instructions) from codebase analysis. |
| LLM tooling | [PromptDiff](https://github.com/he-yufeng/PromptDiff) | new | Semantic diff for LLM prompts: compare prompt versions like `git diff`. |
| LLM tooling | [TokenTracker](https://github.com/he-yufeng/TokenTracker) | new | Drop-in LLM cost tracker: change one import line and see where the money goes. OpenAI, OpenRouter, Azure, Ollama. |
| LLM tooling | [BatchLLM](https://github.com/he-yufeng/BatchLLM) | new | Batch processing for LLM APIs: CSV/JSONL in, results out, with concurrency, retries, checkpointing, and cost tracking. |
| Applied agents | [IslandEscape](https://github.com/he-yufeng/IslandEscape) | new | 2D pixel-art survival game where four LLM agents play the islanders — each with a personality, negotiating trades in natural language and forming alliances; race them to 100 coins to escape. |
| Agent / MCP / CI tooling | [agentcikit](https://github.com/he-yufeng/agentcikit) | new | One CLI for AI-agent, MCP, and open-source work: diagnose CI failures into repro plans, pack issue-specific context for coding agents, gate and replay MCP servers, and test tool-call safety. Bundles `ci-repro`, `patch-context`, `mcp-gate`, `mcp-replay`, and `tool-fence`. |
| Coding agents / evals | [IssueBenchKit](https://github.com/he-yufeng/IssueBenchKit) | new | Turn real GitHub issues and local bugs into small, reproducible coding-agent benchmark tasks with before/after scoring and HTML reports. |
| Agent observability | [FlightBox](https://github.com/he-yufeng/FlightBox) | new | Black-box flight recorder for AI agents: record, redact, replay, and diff local agent sessions. |
| Quant / RL | [DRL-MultiFactorTrading](https://github.com/he-yufeng/DRL-MultiFactorTrading) | new | Deep-RL trading: Double DQN with Transformer attention over a Fama-French-style multi-factor model, plus adaptive risk and volatility targeting. |
| Research | [adversarial-refinement-imputation](https://github.com/he-yufeng/adversarial-refinement-imputation) | new | Companion code for the MiLeTS 2026 paper adapting R3GAN to multivariate time-series imputation — a clearly-scoped negative result. |
| Research | [TrajBias](https://github.com/he-yufeng/TrajBias) | new | A study of structural biases in LLM-as-judge evaluation of agent trajectories. |

### Open Source Contributions

| Project | PR | What I Fixed |
|---------|:--:|-------------|
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5946](https://github.com/QwenLM/qwen-code/pull/5946) | Isolate Anthropic SDK abort listener leak with per-request child controllers |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5020](https://github.com/QwenLM/qwen-code/pull/5020) | Drop tool calls after a cancellation so an aborted turn can't leak stale requests into the next payload. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4829](https://github.com/QwenLM/qwen-code/pull/4829) | Added a timeout to Qwen OAuth refresh so a stalled refresh endpoint can't hang the CLI on auth recovery. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5071](https://github.com/QwenLM/qwen-code/pull/5071) | Submit fast tool results after stream end, so a race at the tail of streaming can't strand completed calls. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#6981](https://github.com/QwenLM/qwen-code/pull/6981) | Route id-less continuation chunks to the colliding tool-call opener's slot instead of dropping them into the wrong one |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4716](https://github.com/QwenLM/qwen-code/pull/4716) | Routed `/bug`, `/docs`, and `/insight` browser launches through the secure opener so headless environments stop crashing on raw `open`. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4622](https://github.com/QwenLM/qwen-code/pull/4622) | Kept assistant tool calls adjacent to their results, so OpenAI-compatible providers stop rejecting repaired histories. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5058](https://github.com/QwenLM/qwen-code/pull/5058) | Stopped stale tool-schema recall from slipping outdated tool names back into later planning turns. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#7535](https://github.com/QwenLM/qwen-code/pull/7535) | Retry model calls with backoff and a circuit breaker in release-notes generation, and surface degraded output instead of a silent blank |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5945](https://github.com/QwenLM/qwen-code/pull/5945) | Reject non-positive sessionRecapAwayThresholdMinutes values |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5429](https://github.com/QwenLM/qwen-code/pull/5429) | Accept uppercase URL schemes when parsing install sources |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5426](https://github.com/QwenLM/qwen-code/pull/5426) | Accept uppercase URL schemes in mcp add transport detection |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5036](https://github.com/QwenLM/qwen-code/pull/5036) | Actually hard-stop repeated identical tool calls once loop detection fires, instead of letting the agent keep hammering the same stalled action. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4970](https://github.com/QwenLM/qwen-code/pull/4970) | Stabilize truncated tool-retry keys so a repaired call keeps the same retry identity instead of drifting. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4673](https://github.com/QwenLM/qwen-code/pull/4673) | Restore top-level `--list-extensions` / `-l` so it prints installed extensions and exits before sandbox, auth, or TUI startup |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5815](https://github.com/QwenLM/qwen-code/pull/5815) | Merging assistant turns was dropping `reasoning_content`, losing multi-turn chain-of-thought. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5070](https://github.com/QwenLM/qwen-code/pull/5070) | Skip expired live agents in focus navigation so stale background-agent rows can't grab keyboard focus. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4639](https://github.com/QwenLM/qwen-code/pull/4639) | Dropped the discontinued Qwen OAuth path from ACP login so nobody gets routed into a dead auth method. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5752](https://github.com/QwenLM/qwen-code/pull/5752) | Parse QWEN_SERVE_MCP_CLIENT_BUDGET strictly as a decimal integer |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5719](https://github.com/QwenLM/qwen-code/pull/5719) | Validate list maxEntries as a positive integer |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5679](https://github.com/QwenLM/qwen-code/pull/5679) | Parse agent & workflow integer env vars strictly |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5647](https://github.com/QwenLM/qwen-code/pull/5647) | Detect USE_OPENAI auth when the model is set via QWEN_MODEL |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5630](https://github.com/QwenLM/qwen-code/pull/5630) | Escape backslashes and quotes in emacs ediff paths |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5494](https://github.com/QwenLM/qwen-code/pull/5494) | Don't treat an empty-parts message as a function call/response |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5461](https://github.com/QwenLM/qwen-code/pull/5461) | Accept uppercase URL schemes in Claude plugin sources |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5420](https://github.com/QwenLM/qwen-code/pull/5420) | Keep estimated token split summing to total |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5336](https://github.com/QwenLM/qwen-code/pull/5336) | Detect WebP and AVI in RIFF magic-byte sniffing |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5328](https://github.com/QwenLM/qwen-code/pull/5328) | Keep qwen3.6-flash and kimi-k2.6 presets text-only |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5287](https://github.com/QwenLM/qwen-code/pull/5287) | Render a sub-minute duration that rounds to 60s as "1m" |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5285](https://github.com/QwenLM/qwen-code/pull/5285) | Confirm the WEBP signature, not just the RIFF prefix |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5227](https://github.com/QwenLM/qwen-code/pull/5227) | Read BMP height as signed int32 for top-down bitmaps |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5194](https://github.com/QwenLM/qwen-code/pull/5194) | Read WebP VP8X canvas height from the correct byte offset |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5209](https://github.com/QwenLM/qwen-code/pull/5209) | Read SHORT-typed TIFF dimensions correctly on big-endian files |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5204](https://github.com/QwenLM/qwen-code/pull/5204) | Reopen code fences without inserting a blank line |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5167](https://github.com/QwenLM/qwen-code/pull/5167) | Hide unconfigured discontinued OAuth model |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5073](https://github.com/QwenLM/qwen-code/pull/5073) | Warn when context instruction files blow the configured budget, before oversized repo guidance quietly crowds out the task. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5115](https://github.com/QwenLM/qwen-code/pull/5115) | Hide teammate-only agent names when teams are disabled and fall back to one-shot subagents if an old prompt still sends one |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5062](https://github.com/QwenLM/qwen-code/pull/5062) | Carry token-escalation context across agent rounds so a delegated run stops restarting from an under-provisioned model each time. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5077](https://github.com/QwenLM/qwen-code/pull/5077) | Show the full plan when a permission gate blocks, so you can inspect the agent's intent instead of losing it. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5061](https://github.com/QwenLM/qwen-code/pull/5061) | Preserve background-agent launch flags so a delegated CLI run keeps the execution mode you asked for. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4963](https://github.com/QwenLM/qwen-code/pull/4963) | Enable fork subagents by default, so delegated work runs in isolated branches without a manual opt-in. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5043](https://github.com/QwenLM/qwen-code/pull/5043) | Let grep results satisfy the prior-read check, so an edit can proceed on verified search context instead of a redundant re-read. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4828](https://github.com/QwenLM/qwen-code/pull/4828) | Keep a user-set shared `baseUrl` after auth refresh, so a same-model refresh doesn't fall back to the provider default. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4715](https://github.com/QwenLM/qwen-code/pull/4715) | Managed auto-memory now honors the runtime output dir, while an explicit memory-dir override still wins. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4596](https://github.com/QwenLM/qwen-code/pull/4596) | Recurse into tracked Git submodules when crawling a repo, so the agent's context picks up files inside them. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4738](https://github.com/QwenLM/qwen-code/pull/4738) | Skip hidden thought parts when copying visible CLI output, so the clipboard matches what's on screen. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4717](https://github.com/QwenLM/qwen-code/pull/4717) | Replace exit-time deep history clones with shallow read paths across copy, arena, and ACP snapshot flows while keeping restore-time cloning defensive |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4600](https://github.com/QwenLM/qwen-code/pull/4600) | Distinguish AUTO from AUTO_EDIT approval-mode indicators in the TUI, including shared styling, i18n keys, and visual evidence |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4636](https://github.com/QwenLM/qwen-code/pull/4636) | Apply the requested output language to side queries too, so auxiliary answers follow the same language contract. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4635](https://github.com/QwenLM/qwen-code/pull/4635) | Hide completed sticky todos from the active CLI view so the list stays on what's left. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4632](https://github.com/QwenLM/qwen-code/pull/4632) | Harden context-error text extraction so a nested or non-string payload surfaces a useful message instead of vanishing. |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4607](https://github.com/QwenLM/qwen-code/pull/4607) | Fix IDE proxy requests by keeping `fetch` and `EnvHttpProxyAgent` on the same bundled `undici` module path |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5072](https://github.com/QwenLM/qwen-code/pull/5072) | Stabilize the simple MCP integration check so server-readiness timing stops making the cross-process contract test flaky. |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#1629](https://github.com/kvcache-ai/Mooncake/pull/1629) | GB200 MNNVL EP hang: `cudaMalloc` → `cuMemCreate(FABRIC)` + `cuMemMap` for cross-node NVLink |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#1644](https://github.com/kvcache-ai/Mooncake/pull/1644) | MNNVL warmup hang: skip redundant handshake for fabric-connected nodes |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2570](https://github.com/kvcache-ai/Mooncake/pull/2570) | Integer overflow in `BatchOffload` for >4 GiB objects: sum slice sizes in `uint64_t` and reject objects exceeding the `uint32_t` record `value_len`, instead of silently truncating |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#3146](https://github.com/kvcache-ai/Mooncake/pull/3146) | Fix double free of UB/Barex slices on device-selection failure: queued slices were deallocated into the cache while `TransferTask` still owned them (sibling of the RDMA fix #3125) |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2965](https://github.com/kvcache-ai/Mooncake/pull/2965) | Roll back partial registration in `registerLocalMemory` on a later transport failure, so earlier transports' registrations don't leak |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#3062](https://github.com/kvcache-ai/Mooncake/pull/3062) | Arm the etcd view-change watch once per wait instead of per iteration, stopping the steady-state watch goroutine leak in HA mode |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#3054](https://github.com/kvcache-ai/Mooncake/pull/3054) | Restore zero-copy puts for multi-buffer payloads in the wheel, which a just-merged refactor had silently regressed into copies |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2628](https://github.com/kvcache-ai/Mooncake/pull/2628) | Fix source refcnt leak in CopyEnd/MoveEnd on invalid source |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#1831](https://github.com/kvcache-ai/Mooncake/pull/1831) | TENT NVLink IPC fix: use base pointer for sub-allocated GPU tensors, porting #1622 fix to TENT path |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#1728](https://github.com/kvcache-ai/Mooncake/pull/1728) | Hard pin for eviction-protected objects: model weights never get evicted, const field + BatchEvict skip + backward-compat serialization |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#1719](https://github.com/kvcache-ai/Mooncake/pull/1719) | Add `ObjectDataType` metadata classification for KV cache, weights, tensors, and snapshots, with backward-compatible serialization and Python bindings |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2610](https://github.com/kvcache-ai/Mooncake/pull/2610) | A refactor had dropped the per-task `request` pointer in `RdmaTransport::submitTransfer`, leaving every downstream task null and breaking status, retry, and accounting reads. Traced it back and restored the association. |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#3278](https://github.com/kvcache-ai/Mooncake/pull/3278) | Block SIGTERM/SIGINT for the graceful-shutdown watcher thread: a process-directed signal landing on the watcher suspended the only pipe reader and hung shutdown forever |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2311](https://github.com/kvcache-ai/Mooncake/pull/2311) | Duplicate `rpc_meta` re-publishes are idempotent when the HTTP body is unchanged, and still rejected when a value actually changes. |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#1825](https://github.com/kvcache-ai/Mooncake/pull/1825) | Fix `P2PClientService::Put` silently swallowing write errors: propagate actual error codes for non-idempotent failures |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2955](https://github.com/kvcache-ai/Mooncake/pull/2955) | Skip the CUDA pointer probe on GPU-less hosts so TransferEngine init succeeds there (the probe result was only ever logged) |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2606](https://github.com/kvcache-ai/Mooncake/pull/2606) | Map cudaStreamQuery for the intra-node NVLink build |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2500](https://github.com/kvcache-ai/Mooncake/pull/2500) | Don't fail bundle cleanup when per-key remove retry succeeds |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2651](https://github.com/kvcache-ai/Mooncake/pull/2651) | Skip bucket files with non-numeric names instead of aborting Init |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2629](https://github.com/kvcache-ai/Mooncake/pull/2629) | Don't abort client init on a malformed MC_MS_AUTO_DISC value |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2460](https://github.com/kvcache-ai/Mooncake/pull/2460) | Support EulerOS in dependencies installer |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2927](https://github.com/kvcache-ai/Mooncake/pull/2927) | Snapshot restore dropped `ssd_total_capacity_bytes`, so SSD total capacity read `0 B` in metrics until the client re-ran `FileStorage::Init`; serialize it with the segment |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2942](https://github.com/kvcache-ai/Mooncake/pull/2942) | Surface HTTP metadata server bind failures in `start()`: it discarded the `async_start()` future, so a bind error (e.g. port in use) stayed invisible and `poll()` reported healthy forever |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2403](https://github.com/kvcache-ai/Mooncake/pull/2403) | Clean up a failed io_uring sub-batch init so a half-prepared transfer batch can't carry broken state into later setup. |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2402](https://github.com/kvcache-ai/Mooncake/pull/2402) | Reject failed Python buddy-allocator backing buffers instead of inserting null raw buffers into managed slabs |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2962](https://github.com/kvcache-ai/Mooncake/pull/2962) | Make single unregisterLocalMemory best-effort so teardown no longer has to track exact registration state |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2627](https://github.com/kvcache-ai/Mooncake/pull/2627) | Guard against null endpoint_store_ in UrmaContext destructor |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2641](https://github.com/kvcache-ai/Mooncake/pull/2641) | Guard MC_TCP_SLICE_SIZE parsing against std::stoull throwing |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2619](https://github.com/kvcache-ai/Mooncake/pull/2619) | Fix signed-char isxdigit UB in EFA smaps page-size parsing (follow-up to #2504) |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2617](https://github.com/kvcache-ai/Mooncake/pull/2617) | Associate task.request in EFA/Kunpeng submitTransfer |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2602](https://github.com/kvcache-ai/Mooncake/pull/2602) | Return HTTP 500 when is_exist reports an error in handle_exist |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#2506](https://github.com/kvcache-ai/Mooncake/pull/2506) | Parse string booleans for enable_ssd_offload in from_file |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#3064](https://github.com/kvcache-ai/Mooncake/pull/3064) | Drop the no-op `enable_mooncake_nof_pool` key from the NVMe-oF docs so users stop copying a setting that does nothing |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#1626](https://github.com/kvcache-ai/Mooncake/pull/1626) | Silenced error log spam for non-memory replicas in metadata store |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · maintainer) | [#3266](https://github.com/kvcache-ai/Mooncake/pull/3266) | Poll for the async eviction in PutStartExpiringTest instead of asserting right away, killing a timing flake in CI |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#7196](https://github.com/AstrBotDevs/AstrBot/pull/7196) | Fix Gemini thinking parts leaking into user-facing response |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#6474](https://github.com/AstrBotDevs/AstrBot/pull/6474) | SQLite `database is locked` under concurrent writes: added busy timeout |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#6596](https://github.com/AstrBotDevs/AstrBot/pull/6596) | Multimodal token counting: images, audio, chain-of-thought were invisible to context compression |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#7537](https://github.com/AstrBotDevs/AstrBot/pull/7537) | Prevent Telegram media group exceptions from being silently swallowed by APScheduler |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#7758](https://github.com/AstrBotDevs/AstrBot/pull/7758) | Apply empty-assistant message filter to streaming OpenAI path: strict providers no longer 400 on reasoning-only turns |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8736](https://github.com/AstrBotDevs/AstrBot/pull/8736) | Preserve embedding API version suffixes so a versioned provider endpoint doesn't get normalized to the wrong path. |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8750](https://github.com/AstrBotDevs/AstrBot/pull/8750) | Fixed changelog anchor links so dashboard release notes jump to the right section instead of a dead anchor. |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8388](https://github.com/AstrBotDevs/AstrBot/pull/8388) | Add the missing dashboard i18n for plugin sub-command counts, so extension details stop showing raw translation keys. |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8175](https://github.com/AstrBotDevs/AstrBot/pull/8175) | Surface WeChat OA media send failures instead of reporting success after prepare/send timeouts |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8255](https://github.com/AstrBotDevs/AstrBot/pull/8255) | Support RST and AsciiDoc knowledge uploads by keeping backend parser checks and dashboard file validation in sync |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#7398](https://github.com/AstrBotDevs/AstrBot/pull/7398) | Fix Telegram sendMessageDraft spamming 400 errors on empty text in streaming mode |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#7217](https://github.com/AstrBotDevs/AstrBot/pull/7217) | Fix qwen3-rerank response parsing: handle both old and new Dashscope API formats |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8768](https://github.com/AstrBotDevs/AstrBot/pull/8768) | Sanitize Lark platform id suffixes so invisible whitespace in configured ids does not break platform matching |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8718](https://github.com/AstrBotDevs/AstrBot/pull/8718) | Avoid duplicate quoted image captions when multimodal replies include both quoted text and image metadata |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8172](https://github.com/AstrBotDevs/AstrBot/pull/8172) | Prefer bundled dashboard assets over a stale data dist, so a release stops serving an outdated WebUI. |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#6710](https://github.com/AstrBotDevs/AstrBot/pull/6710) | Skills-like re-query dropping image captions: `extra_user_content_parts` not forwarded |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#6581](https://github.com/AstrBotDevs/AstrBot/pull/6581) | Context truncation dropping the only user message: causes 400 from Zhipu/Gemini |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8786](https://github.com/AstrBotDevs/AstrBot/pull/8786) | Enforce persona tool boundaries |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8089](https://github.com/AstrBotDevs/AstrBot/pull/8089) | Route image requests to a vision-capable fallback provider when the primary provider cannot accept image input |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8195](https://github.com/AstrBotDevs/AstrBot/pull/8195) | Skip empty LLM summaries so context compression keeps the original history instead of inserting a blank placeholder. |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8119](https://github.com/AstrBotDevs/AstrBot/pull/8119) | Pass image inputs through active replies so image-triggered mentions reach the LLM as image URLs |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8061](https://github.com/AstrBotDevs/AstrBot/pull/8061) | Keep Discord startup alive when command sync hits the daily create quota; only quota errors become warnings |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8073](https://github.com/AstrBotDevs/AstrBot/pull/8073) | Fix image-only KB retrieval: skip blank prompts so embedding APIs are not called with empty text |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#7407](https://github.com/AstrBotDevs/AstrBot/pull/7407) | Fix Gemini native search 400 when no function tools: skip FunctionCallingConfig |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#7216](https://github.com/AstrBotDevs/AstrBot/pull/7216) | Fix Gemini tool call 400: wrap plain-text tool results as Protobuf Struct |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#6551](https://github.com/AstrBotDevs/AstrBot/pull/6551) | Fix empty content causing Grok 400: set content to None when empty |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#7003](https://github.com/AstrBotDevs/AstrBot/pull/7003) | SSE heartbeat for WebChat: long context compression killed the connection |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#6656](https://github.com/AstrBotDevs/AstrBot/pull/6656) | `/stop` follow-up race: agent_stop flag not checked during follow-up capture |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#6527](https://github.com/AstrBotDevs/AstrBot/pull/6527) | Fix LLM tool selection: rewrote ambiguous Upload/Download descriptions |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#6313](https://github.com/AstrBotDevs/AstrBot/pull/6313) | Null choices guard: OpenAI API returning `None` instead of empty list |
| [OpenClaw](https://github.com/openclaw/openclaw) (385.5k★) | [#119127](https://github.com/openclaw/openclaw/pull/119127) | Keep the mtime media sweep out of the managed-outgoing tree and fail closed when the session store is unreadable, so global GC can never delete live user originals (co-built with the project owner after his P0 review) |
| [OpenClaw](https://github.com/openclaw/openclaw) (385.5k★) | [#41271](https://github.com/openclaw/openclaw/pull/41271) | Log auth profile resolution failures instead of swallowing silently |
| [OpenClaw](https://github.com/openclaw/openclaw) (385.5k★) | [#41259](https://github.com/openclaw/openclaw/pull/41259) | Propagate memory directory creation failures instead of continuing after a failed `ensureDir` |
| [OpenClaw](https://github.com/openclaw/openclaw) (385.5k★) | [#106603](https://github.com/openclaw/openclaw/pull/106603) | Use the canonical `shortenHomePath` in the sandbox-root escape error so the reported path matches the rest of the UI. |
| [OpenClaw](https://github.com/openclaw/openclaw) (385.5k★) | [#96562](https://github.com/openclaw/openclaw/pull/96562) | Keep sibling dirs that share the home prefix unshortened in tool path display |
| [OpenClaw](https://github.com/openclaw/openclaw) (385.5k★) | [#96456](https://github.com/openclaw/openclaw/pull/96456) | Clip progress text on code-point boundaries to avoid lone surrogates |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#37884](https://github.com/vllm-project/vllm/pull/37884) | RoBERTa's in-place `position_ids` accumulation bled into CUDA-graph padding, crashing BGE-M3 after ~4k requests. |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#37727](https://github.com/vllm-project/vllm/pull/37727) | Responses API `instructions` were leaking across turns through the `previous_response_id` chain. |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#40789](https://github.com/vllm-project/vllm/pull/40789) | Taught the V1 ubatch wrapper to unwrap tuple model outputs, unblocking DBO and speculative decoding on tuple-returning models. |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#43243](https://github.com/vllm-project/vllm/pull/43243) | Qwen3 XML tool-call params now parse as JSON first, so `null`/`false` survive streaming instead of being rejected as Python literals. |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#44821](https://github.com/vllm-project/vllm/pull/44821) | Prefix DeepSeek V4 MTP projection layers so compressed-tensors can match artifact-side target and ignore rules during draft model loading |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#42679](https://github.com/vllm-project/vllm/pull/42679) | Guard flash-attn rotary imports so FA4 environments fall back cleanly when `flash_attn.ops.triton.rotary` is absent |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#38732](https://github.com/vllm-project/vllm/pull/38732) | Fix bench_serve UTF-8 decode crash on split multi-byte chars in streaming chunks |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#37699](https://github.com/vllm-project/vllm/pull/37699) | Fix weight offloading ignoring `VLLM_WEIGHT_OFFLOADING_DISABLE_PIN_MEMORY` in prefetch offloader |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#37301](https://github.com/vllm-project/vllm/pull/37301) | Base64 JPEG video frames returning empty metadata: populate frame count, fps, duration |
| [PyTorch](https://github.com/pytorch/pytorch) (102.3k★) | [#188229](https://github.com/pytorch/pytorch/pull/188229) | `avg_pool3d` backward silently corrupted gradients on inputs over `INT_MAX` elements: the atomic scatter kernel computed offsets and bounds as 32-bit `int`; widened to 64-bit indexing (shows as Closed; landed via pytorchmergebot) |
| [PyTorch](https://github.com/pytorch/pytorch) (102.3k★) | [#188022](https://github.com/pytorch/pytorch/pull/188022) | Guard the CuTeDSL topk override against a non-current CUDA device so it stops dispatching on the wrong device (shows as Closed; landed via pytorchmergebot) |
| [PyTorch](https://github.com/pytorch/pytorch) (102.3k★) | [#186779](https://github.com/pytorch/pytorch/pull/186779) | Error on unsupported batch norm third derivatives instead of silently returning wrong gradients (shows as Closed; landed via pytorchmergebot) |
| [PyTorch](https://github.com/pytorch/pytorch) (102.3k★) | [#188027](https://github.com/pytorch/pytorch/pull/188027) | Initialize `r` in the Laguerre and Legendre polynomial helpers so they stop returning uninitialized memory on the boundary path (shows as Closed; landed via pytorchmergebot) |
| [PyTorch](https://github.com/pytorch/pytorch) (102.3k★) | [#187860](https://github.com/pytorch/pytorch/pull/187860) | Route the empty-`src` check in `meta__transformer_encoder_layer_fwd` through `guard_or_false` so an unbacked symbolic `numel` under `torch.compile` no longer raises a data-dependent error (shows as Closed; landed via pytorchmergebot) |
| [PyTorch](https://github.com/pytorch/pytorch) (102.3k★) | [#176100](https://github.com/pytorch/pytorch/pull/176100) | Fix user-defined Triton kernel name mangling in the Inductor codegen so distinct kernels stop colliding in generated code (shows as Closed; landed via pytorchmergebot) |
| [PyTorch](https://github.com/pytorch/pytorch) (102.3k★) | [#187643](https://github.com/pytorch/pytorch/pull/187643) | Fix a `ValueError` in the `stale_issues` workflow's `parse_older_than` on non-leap years, where a naive Feb 29 offset crashed the run (shows as Closed; landed via pytorchmergebot) |
| [PyTorch](https://github.com/pytorch/pytorch) (102.3k★) | [#187262](https://github.com/pytorch/pytorch/pull/187262) | Remove the obsolete `setuptools` upper bound so builds resolve a current toolchain instead of pinning a stale one (shows as Closed; landed via pytorchmergebot) |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#3797](https://github.com/bytedance/deer-flow/pull/3797) | Synchronize the MCP session-pool singleton lifecycle so concurrent first-use cannot create duplicate pools |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#3799](https://github.com/bytedance/deer-flow/pull/3799) | Serialize per-chat thread creation so concurrent messages stop spawning duplicate threads for one chat. |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#3800](https://github.com/bytedance/deer-flow/pull/3800) | Keep `create_thread` idempotent when a concurrent insert loses the race, so a chat cannot end up with duplicate threads. |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#4157](https://github.com/bytedance/deer-flow/pull/4157) | A subagent's `description` is agent-editable (setup_agent / update_agent) yet was rendered raw into the `<subagent_system>` block, so a crafted first line could break out and forge framework tags. Escaped it, matching the `<soul>` fix. |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#4137](https://github.com/bytedance/deer-flow/pull/4137) | HTML-escape `SOUL.md` before it enters the `<soul>` system-prompt block so an agent-editable personality cannot forge framework tags and break out of its trust zone |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#3778](https://github.com/bytedance/deer-flow/pull/3778) | Synchronize skill storage singleton lifecycle |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#3631](https://github.com/bytedance/deer-flow/pull/3631) | Strip base64 image data from streamed values events |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#4216](https://github.com/bytedance/deer-flow/pull/4216) | `get_memory_config()` only refreshed as a side effect of `get_app_config()`, so readers like the agent factory saw a stale `memory.mode` after a config.yaml edit; resolve through `get_app_config()` with a FileNotFoundError fallback |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#4429](https://github.com/bytedance/deer-flow/pull/4429) | Fork-restored checkpoints deliver the sandbox channel still wrapped in langgraph `Overwrite`; unified one unwrap helper across the sync/async init paths and the sibling readers |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#4381](https://github.com/bytedance/deer-flow/pull/4381) | Unwrap Overwrite-wrapped sandbox state in after_agent so hook consumers read the real state instead of the wrapper |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#4253](https://github.com/bytedance/deer-flow/pull/4253) | A tool result containing a literal `</tool_response>` could close the MindIE framing early and inject trailing text; escaped the tool-response content, matching the tool-call name/arg escaping already in the same function. |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#4130](https://github.com/bytedance/deer-flow/pull/4130) | Recognize remaining requests/httpx HTTP methods as network sinks |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#3674](https://github.com/bytedance/deer-flow/pull/3674) | Let UI runtime channel config win over config.yaml |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#3719](https://github.com/bytedance/deer-flow/pull/3719) | Skip whitespace-only facts in `_apply_updates` so blank memory entries do not accumulate |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#3709](https://github.com/bytedance/deer-flow/pull/3709) | Fix positional fallback consuming unrelated todo when same-content list is exhausted |
| [Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) (30.3k★ · maintainer) | [#777](https://github.com/HKUDS/Vibe-Trading/pull/777) | Portfolio Studio's risk x-ray: pure-computation concentration, volatility, drawdown, VaR/ES, diversification, and correlation analytics for weighted baskets, plus an agent tool that fetches closes through the loader fallback chain |
| [Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) (30.3k★ · maintainer) | [#900](https://github.com/HKUDS/Vibe-Trading/pull/900) | Every backtest run now emits a risk x-ray artifact (JSON + Markdown) over the strategy's average basket, with concentration, volatility, drawdown, and tail-risk metrics folded into run metrics |
| [Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) (30.3k★ · maintainer) | [#818](https://github.com/HKUDS/Vibe-Trading/pull/818) | Portfolio Studio step 2: composable weight constraints that plug into any optimizer, with waterfill redistribution that only feeds positions still under their cap |
| [Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) (30.3k★ · maintainer) | [#796](https://github.com/HKUDS/Vibe-Trading/pull/796) | Wired the strict alpha-bench gate into the CLI: `alpha bench --strict` now fails the run when a strategy misses the bar |
| [Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) (30.3k★ · maintainer) | [#795](https://github.com/HKUDS/Vibe-Trading/pull/795) | Portfolio Studio's rebalance notes: the backtester now writes a notes artifact with metrics for each rebalance, so agent-driven moves stay auditable |
| [Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) (30.3k★ · maintainer) | [#966](https://github.com/HKUDS/Vibe-Trading/pull/966) | Surface Portfolio Studio artifacts in run detail, so risk x-ray and rebalance outputs show up where a run is inspected |
| [Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) (30.3k★ · maintainer) | [#970](https://github.com/HKUDS/Vibe-Trading/pull/970) | Route `source: yfinance` crypto backtests to CryptoEngine instead of the stock path, so BTC/ETH runs stop erroring out |
| [Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) (30.3k★ · maintainer) | [#984](https://github.com/HKUDS/Vibe-Trading/pull/984) | Write hierarchy-routed memory entries with the .md extension so discovery actually sees them (bare-slug files were invisible to list/recall) |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5808](https://github.com/microsoft/agent-framework/pull/5808) | Handoff was mutating message roles in place, so a retry leaked the change; reuse sanitized copies instead. |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5462](https://github.com/microsoft/agent-framework/pull/5462) | Fix `background=True` + tools infinite-retrieve loop: clear completed continuation state so tool results get posted |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5773](https://github.com/microsoft/agent-framework/pull/5773) | Run synchronous Python tools off the event loop so a blocking call stops freezing concurrent agent work. |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5815](https://github.com/microsoft/agent-framework/pull/5815) | Forward MCP `tools/list` metadata into `call_tool` instrumentation so traces keep their tool annotations. |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5801](https://github.com/microsoft/agent-framework/pull/5801) | Coalesce streamed code-interpreter history by call id, so stored history keeps the full code and results without duplicated deltas. |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#7162](https://github.com/microsoft/agent-framework/pull/7162) | Python: Anthropic streaming counted token usage twice by accumulating final-message usage on top of streamed deltas |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#6132](https://github.com/microsoft/agent-framework/pull/6132) | Filter filesystem checkpoint indexes by session id, so reopening a store stops returning another session's checkpoints. |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5904](https://github.com/microsoft/agent-framework/pull/5904) | Keep ChatClientAgent's local history provider on for AG-UI thread ids, so session history isn't mistaken for service-managed model history. |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5976](https://github.com/microsoft/agent-framework/pull/5976) | Fix sequential workflow sample output so all participant responses are shown from non-streaming results |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5799](https://github.com/microsoft/agent-framework/pull/5799) | Add handoff workflow naming metadata so names and descriptions flow through builder and hosting registration |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#7256](https://github.com/microsoft/agent-framework/pull/7256) | Python: `from_dict` validated a payload's self-declared `type` against itself, so the check could never fail; resolve the expected type from the class instead |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#7108](https://github.com/microsoft/agent-framework/pull/7108) | Python: `FunctionTool.invoke` dumped arguments with `exclude_none=True`, dropping deliberate `null` values for required nullable parameters; use `exclude_unset` so explicit nulls survive |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#6210](https://github.com/microsoft/agent-framework/pull/6210) | Drop hosted MCP tool-call history when reasoning payloads are stripped, so stateless OpenAI replay stops sending orphan MCP calls. |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5861](https://github.com/microsoft/agent-framework/pull/5861) | Foundry handoff arguments were losing their structure in response conversion, breaking delegated agent calls; preserved them. |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#7239](https://github.com/microsoft/agent-framework/pull/7239) | Python: AG-UI MESSAGES_SNAPSHOT emitted messages out of the model's original order; preserve emission order |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#7130](https://github.com/microsoft/agent-framework/pull/7130) | Python: extract keywords from non-English text for topic selection, so CJK and other non-latin queries stop coming back empty |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#7124](https://github.com/microsoft/agent-framework/pull/7124) | Python: compaction token counting serialized messages with `ensure_ascii=True`, so the tokenizer counted `\uXXXX` escapes instead of real characters (~1.6x inflation on CJK); serialize the real text |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#6640](https://github.com/microsoft/agent-framework/pull/6640) | Python: surface cache and reasoning token counts for the Bedrock and Gemini connectors |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#6491](https://github.com/microsoft/agent-framework/pull/6491) | .NET: fix fan-in barrier checkpoint state |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#6208](https://github.com/microsoft/agent-framework/pull/6208) | Declarative `Foreach` was collapsing multi-field PowerFx table rows; preserve the full record value through iteration. |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5784](https://github.com/microsoft/agent-framework/pull/5784) | Skip orphan Anthropic thinking signatures when converting history, so a replay doesn't carry an invalid standalone signature. |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#6040](https://github.com/microsoft/agent-framework/pull/6040) | Forward a Foundry agent's `default_headers` into OpenAI client creation, so custom auth and routing headers survive setup. |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#6037](https://github.com/microsoft/agent-framework/pull/6037) | Keep Foundry citation `get_url` metadata through response conversion so source links survive in chat responses |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5974](https://github.com/microsoft/agent-framework/pull/5974) | Include Foundry agent tool definitions in eval mappings so evaluator runs can call code-defined tools |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5800](https://github.com/microsoft/agent-framework/pull/5800) | Avoid AG-UI tool result message id collisions when providers omit update ids |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5778](https://github.com/microsoft/agent-framework/pull/5778) | Declare the Magentic protocol messages so orchestrator chat/reset signals deserialize instead of blowing up on an unknown type. |
| [opencode](https://github.com/anomalyco/opencode) (195.0k★) | [#30022](https://github.com/anomalyco/opencode/pull/30022) | Bind the MCP OAuth callback server to the IPv4 loopback so the browser redirect connects reliably instead of racing IPv6 |
| [dify](https://github.com/langgenius/dify) (151.8k★) | [#39953](https://github.com/langgenius/dify/pull/39953) | Bound the TiDB Cloud API calls that had no timeout, so a hanging cluster endpoint can't stall vdb operations forever |
| [dify](https://github.com/langgenius/dify) (151.8k★) | [#37425](https://github.com/langgenius/dify/pull/37425) | Bound OperationService billing requests so a slow billing endpoint can't hang the request. |
| [dify](https://github.com/langgenius/dify) (151.8k★) | [#39479](https://github.com/langgenius/dify/pull/39479) | Make the 10-minute email IP first-strike window actually take effect: claim the slot atomically with SET NX instead of a racy GET-then-SETEX |
| [dify](https://github.com/langgenius/dify) (151.8k★) | [#38801](https://github.com/langgenius/dify/pull/38801) | Validate the conversation up front on the service-api and explore endpoints, so a bad `conversation_id` returns 404 instead of streaming into a late failure. |
| [dify](https://github.com/langgenius/dify) (151.8k★) | [#37685](https://github.com/langgenius/dify/pull/37685) | Keep watercrawl request timeouts bounded instead of disabling them with `timeout=None` |
| [dify](https://github.com/langgenius/dify) (151.8k★) | [#37669](https://github.com/langgenius/dify/pull/37669) | Skip empty tool entries in legacy dataset config extraction |
| [Transformers](https://github.com/huggingface/transformers) (163.5k★) | [#44710](https://github.com/huggingface/transformers/pull/44710) | `AutoProcessor.from_pretrained` was silently dropping hub kwargs like `revision` and `token`. |
| [OpenHands](https://github.com/OpenHands/OpenHands) (83.5k★) | [#14776](https://github.com/OpenHands/OpenHands/pull/14776) | Keep a custom LLM base URL when editing basic model settings, so a saved profile stops silently falling back to the provider default. |
| [Firecrawl](https://github.com/firecrawl/firecrawl) (163.2k★) | [#3730](https://github.com/firecrawl/firecrawl/pull/3730) | Reject self-hosted scrape interact actions with a clear error instead of failing opaquely |
| [Firecrawl](https://github.com/firecrawl/firecrawl) (163.2k★) | [#3729](https://github.com/firecrawl/firecrawl/pull/3729) | Keep the auth chunk in the self-host bypass path so authenticated self-hosted scrapes don't get dropped. |
| [Firecrawl](https://github.com/firecrawl/firecrawl) (163.2k★) | [#3713](https://github.com/firecrawl/firecrawl/pull/3713) | Handle the async v1 batch-scrape response returned as a dict in the Python SDK |
| [SGLang](https://github.com/sgl-project/sglang) (31.5k★) | [#20739](https://github.com/sgl-project/sglang/pull/20739) | Fix hybrid_linear_attn_backend crash when used with ngram speculative decoding |
| [SGLang](https://github.com/sgl-project/sglang) (31.5k★) | [#21472](https://github.com/sgl-project/sglang/pull/21472) | Fix PicklingError with --backend diffusers on non-T2I models |
| [DeepSpeed](https://github.com/deepspeedai/DeepSpeed) (42.9k★) | [#8049](https://github.com/deepspeedai/DeepSpeed/pull/8049) | Eigenvalue monitor values were computed but never logged; wired them through so they actually land in the record. |
| [Triton](https://github.com/triton-lang/triton) (19.9k★) | [#10883](https://github.com/triton-lang/triton/pull/10883) | Promote fp8 operands before division and modulo instead of evaluating them in fp8 precision (BC breaking) |
| [Triton](https://github.com/triton-lang/triton) (19.9k★) | [#10689](https://github.com/triton-lang/triton/pull/10689) | Keep at least one config when a fractional top_k rounds to zero |
| [Triton](https://github.com/triton-lang/triton) (19.9k★) | [#10687](https://github.com/triton-lang/triton/pull/10687) | `is_power_of_two(0)` was returning True. |
| [Triton](https://github.com/triton-lang/triton) (19.9k★) | [#9613](https://github.com/triton-lang/triton/pull/9613) | Fix AxisInfo correctness: signed constants, unknown shift divisibility, and shift UB guards |
| [Cline](https://github.com/cline/cline) (65.9k★) | [#11166](https://github.com/cline/cline/pull/11166) | Keep file search working when the open-tabs host RPC is down by falling back to system `rg`. |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1822](https://github.com/agentscope-ai/agentscope/pull/1822) | Add a cwd option to the built-in Bash tool so shell commands can run in the intended workspace directory |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1823](https://github.com/agentscope-ai/agentscope/pull/1823) | Add workspace roots to the permission context, so a chat run authorizes files against the workspace the agent can actually see. |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1815](https://github.com/agentscope-ai/agentscope/pull/1815) | Inherit the leader's permission rules in team runs, so delegated agents keep the same workspace and file-access limits. |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1734](https://github.com/agentscope-ai/agentscope/pull/1734) | Refresh Redis message-list TTL on append and streaming replace, so the configured storage TTL actually bounds chat history. |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1786](https://github.com/agentscope-ai/agentscope/pull/1786) | Keep a caller-provided Redis session id on create, so later get/update/list hit the same session instead of a fresh UUID. |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1717](https://github.com/agentscope-ai/agentscope/pull/1717) | Hide Bash tool subprocess windows on Windows with `CREATE_NO_WINDOW`, while leaving non-Windows process creation unchanged |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1883](https://github.com/agentscope-ai/agentscope/pull/1883) | Handle Gemini function calls without an id |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1774](https://github.com/agentscope-ai/agentscope/pull/1774) | Forward explicitly configured Qwen `thinking_enable` into OpenAI-compatible `extra_body` without polluting normal OpenAI requests |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1732](https://github.com/agentscope-ai/agentscope/pull/1732) | Pull skills from every active tool group, so prompt instructions and the Skill viewer match the enabled tools. |
| [LiteLLM](https://github.com/BerriAI/litellm) (55.9k★) | [#26401](https://github.com/BerriAI/litellm/pull/26401) | Fix `LITELLM_LOG=INFO` missing `verbose_logger`: proxy INFO logs now include all verbose logger sources |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#10089](https://github.com/promptfoo/promptfoo/pull/10089) | Reject out-of-range trace-span-duration percentiles instead of silently computing garbage |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9850](https://github.com/promptfoo/promptfoo/pull/9850) | Score tokenless GLEU inputs as zero instead of crashing |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#10124](https://github.com/promptfoo/promptfoo/pull/10124) | Avoid a crash on an empty completion `choices` array in the Azure provider |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#10076](https://github.com/promptfoo/promptfoo/pull/10076) | A tool-call assertion crashed with a TypeError when the tool call was missing its `function` object; return `pass:false` instead. |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9867](https://github.com/promptfoo/promptfoo/pull/9867) | Avoid crashing on an empty `choices` array when reading Azure logprobs |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9897](https://github.com/promptfoo/promptfoo/pull/9897) | Guard array access in the Bedrock Titan and Cohere providers so an empty response array stops crashing generation. |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9815](https://github.com/promptfoo/promptfoo/pull/9815) | Reject a malformed `__expected0` CSV header instead of silently dropping its assertion |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9824](https://github.com/promptfoo/promptfoo/pull/9824) | Correct the inverse-JSON assertion failure messages so they no longer read backwards |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9841](https://github.com/promptfoo/promptfoo/pull/9841) | Return pass:false for empty output instead of throwing |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9840](https://github.com/promptfoo/promptfoo/pull/9840) | Preserve JSONL row description instead of overwriting |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9761](https://github.com/promptfoo/promptfoo/pull/9761) | Preserve quoted commas in contains-any/all assertion values |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9822](https://github.com/promptfoo/promptfoo/pull/9822) | Keep ellipsize within maxLen when maxLen is below 3 |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9757](https://github.com/promptfoo/promptfoo/pull/9757) | Unescape all escaped commas in array metadata values |
| [goose](https://github.com/aaif-goose/goose) (52.6k★) | [#9528](https://github.com/aaif-goose/goose/pull/9528) | Restore new-chat keyboard shortcut navigation in the desktop app |
| [goose](https://github.com/aaif-goose/goose) (52.6k★) | [#9599](https://github.com/aaif-goose/goose/pull/9599) | Use a blocking OTLP HTTP exporter so telemetry isn't lost when the process exits. |
| [goose](https://github.com/aaif-goose/goose) (52.6k★) | [#9584](https://github.com/aaif-goose/goose/pull/9584) | Show resolved skill supporting-file paths instead of unresolved placeholders |
| [GitHub MCP Server](https://github.com/github/github-mcp-server) (32.1k★) | [#2514](https://github.com/github/github-mcp-server/pull/2514) | Support team reviewers in PR review requests by resolving team slugs to review subjects instead of dropping them. |
| [GitHub MCP Server](https://github.com/github/github-mcp-server) (32.1k★) | [#2612](https://github.com/github/github-mcp-server/pull/2612) | Hide write-side UI resources when the MCP server runs read-only, while keeping safe read-only resources registered |
| [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) (28.5k★) | [#3643](https://github.com/openai/openai-agents-python/pull/3643) | Report the effective Blaxel timeouts instead of the unconfigured defaults |
| [ms-swift](https://github.com/modelscope/ms-swift) (15.1k★) | [#9642](https://github.com/modelscope/ms-swift/pull/9642) | Empty `rejected_messages` now fail fast in dataset prep instead of crashing DPO mid-training. |
| [ms-swift](https://github.com/modelscope/ms-swift) (15.1k★) | [#9816](https://github.com/modelscope/ms-swift/pull/9816) | `swift sample` crashed engine construction when `engine_kwargs` carried `torch_dtype` (the workaround while the flag was ignored); pop it before the splat so the flag always wins |
| [ms-swift](https://github.com/modelscope/ms-swift) (15.1k★) | [#9750](https://github.com/modelscope/ms-swift/pull/9750) | A 0-fps `get_avg_fps()` on broken video metadata made `range(0, len(vr), 0)` raise before any frame was read in MiniCPM-V / mPLUG-Owl3 sampling; guard the sample step |
| [ms-swift](https://github.com/modelscope/ms-swift) (15.1k★) | [#9605](https://github.com/modelscope/ms-swift/pull/9605) | Different-format images collided in the temp image cache; folded mode and size into the key. |
| [ms-swift](https://github.com/modelscope/ms-swift) (15.1k★) | [#9612](https://github.com/modelscope/ms-swift/pull/9612) | `_replace_system` was flattening non-string prefix elements, stripping the structured content out of templated system prompts. |
| [ms-swift](https://github.com/modelscope/ms-swift) (15.1k★) | [#9789](https://github.com/modelscope/ms-swift/pull/9789) | Refresh wandb in the CUDA test container setup, unbreaking the repo-wide CI an old baked wandb had poisoned against protobuf 7.x |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1735](https://github.com/ag-ui-protocol/ag-ui/pull/1735) | Avoid stale ADK session writes after human-in-the-loop tool calls |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1890](https://github.com/ag-ui-protocol/ag-ui/pull/1890) | Cache ADK session reads within one execution, so a remote session service isn't refetched before every agent run. |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1828](https://github.com/ag-ui-protocol/ag-ui/pull/1828) | Detect Strands' private session manager so AG-UI history replay respects an active session instead of replaying prior turns. |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1889](https://github.com/ag-ui-protocol/ag-ui/pull/1889) | Collect output-schema agents when building ADK workflow graphs, so structured-output nodes don't get dropped. |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1848](https://github.com/ag-ui-protocol/ag-ui/pull/1848) | Bundle replayed tool results |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1730](https://github.com/ag-ui-protocol/ag-ui/pull/1730) | Allow CopilotKit 1.x runtime peer |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1826](https://github.com/ag-ui-protocol/ag-ui/pull/1826) | Forward LangGraph runtime context through tool kwargs so graph tools keep the caller's execution context. |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1832](https://github.com/ag-ui-protocol/ag-ui/pull/1832) | Preserve AG-UI input metadata when LangGraph converts text and media blocks into LangChain multimodal content |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1829](https://github.com/ag-ui-protocol/ag-ui/pull/1829) | Close LangGraph text messages before tool-call chunks so text-to-tool transitions keep both message and tool events |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1769](https://github.com/ag-ui-protocol/ag-ui/pull/1769) | Make proto generation cross-platform: replace Unix-only `mkdir -p` with a Node script and Windows `.CMD` plugin shim |
| [cherry-studio](https://github.com/CherryHQ/cherry-studio) (50.1k★) | [#16352](https://github.com/CherryHQ/cherry-studio/pull/16352) | Preserve surrogate pairs at truncation boundaries so a multi-byte character isn't split into invalid halves. |
| [cherry-studio](https://github.com/CherryHQ/cherry-studio) (50.1k★) | [#17106](https://github.com/CherryHQ/cherry-studio/pull/17106) | Count images nested in `tool_result` blocks when estimating API-gateway token usage, so multimodal tool results are no longer under-counted |
| [cherry-studio](https://github.com/CherryHQ/cherry-studio) (50.1k★) | [#16358](https://github.com/CherryHQ/cherry-studio/pull/16358) | Drop Ideogram `data[]` items without a usable URL in the aihubmix path instead of rendering broken images |
| [cherry-studio](https://github.com/CherryHQ/cherry-studio) (50.1k★) | [#16454](https://github.com/CherryHQ/cherry-studio/pull/16454) | Keep bare-URL markdown reference lines in citations instead of dropping them |
| [cherry-studio](https://github.com/CherryHQ/cherry-studio) (50.1k★) | [#16361](https://github.com/CherryHQ/cherry-studio/pull/16361) | Resolve the .d.ts icon for uppercase extensions |
| [cherry-studio](https://github.com/CherryHQ/cherry-studio) (50.1k★) | [#16217](https://github.com/CherryHQ/cherry-studio/pull/16217) | Roll relative time up at the unit boundary |
| [Google ADK](https://github.com/google/adk-python) (21.0k★) | [#5698](https://github.com/google/adk-python/pull/5698) | Include intermediate responses in `final_response_match_v2` judging when the criterion opts in |
| [Mem0](https://github.com/mem0ai/mem0) (62.8k★) | [#5380](https://github.com/mem0ai/mem0/pull/5380) | Expose Qdrant's `https` option so a self-hosted HTTP cluster can use API-key auth without being forced into TLS client mode. |
| [Mem0](https://github.com/mem0ai/mem0) (62.8k★) | [#5416](https://github.com/mem0ai/mem0/pull/5416) | Use valid S3 Vectors entity index names so agent memory writes no longer hit AWS index-name validation failures |
| [Mem0](https://github.com/mem0ai/mem0) (62.8k★) | [#5383](https://github.com/mem0ai/mem0/pull/5383) | Skip OpenClaw runtime setup during CLI metadata registration, so plugin discovery stops double-registering runtime side effects. |
| [verl](https://github.com/verl-project/verl) (22.9k★) | [#6620](https://github.com/verl-project/verl/pull/6620) | Derived the colocated vLLM weight-sync ZMQ socket rank from the DP and TP ranks, so DP workers stop colliding on one receiver. |
| [TRL](https://github.com/huggingface/trl) (19.0k★) | [#6054](https://github.com/huggingface/trl/pull/6054) | An already-transformed dataset in SFT prep now fails fast, instead of silently producing wrong training batches. |
| [TRL](https://github.com/huggingface/trl) (19.0k★) | [#6063](https://github.com/huggingface/trl/pull/6063) | Preserve vllm prompt special tokens |
| [Agno](https://github.com/agno-agi/agno) (41.6k★) | [#8131](https://github.com/agno-agi/agno/pull/8131) | Preserve non-sentinel tool argument whitespace while keeping string-to-None/True/False normalization for exact sentinels |
| [RAGFlow](https://github.com/infiniflow/ragflow) (87.1k★) | [#15691](https://github.com/infiniflow/ragflow/pull/15691) | Skip empty agent-switch conditions so a blank branch guard can't crash or block valid downstream flows. |
| [RAGFlow](https://github.com/infiniflow/ragflow) (87.1k★) | [#15696](https://github.com/infiniflow/ragflow/pull/15696) | Keep the strongest PageRank score for repeated n-hop GraphRAG edges, so path order can't overwrite the ranking. |
| [RAGFlow](https://github.com/infiniflow/ragflow) (87.1k★) | [#15601](https://github.com/infiniflow/ragflow/pull/15601) | Fall back when Docling native parsing returns no chunks, so a document still produces usable content instead of an empty parse. |
| [LiveKit Agents](https://github.com/livekit/agents) (12.7k★) | [#5864](https://github.com/livekit/agents/pull/5864) | Surface Soniox STT server errors instead of treating failed streams as empty transcripts |
| [LiveKit Agents](https://github.com/livekit/agents) (12.7k★) | [#5820](https://github.com/livekit/agents/pull/5820) | Recreate Anthropic streaming requests on retry so transient stream creation failures do not re-await the same coroutine |
| [LiveKit Agents](https://github.com/livekit/agents) (12.7k★) | [#5994](https://github.com/livekit/agents/pull/5994) | Handle OpenAI-compatible realtime status details that come back as strings, so an incomplete response doesn't crash logging. |
| [LiveKit Agents](https://github.com/livekit/agents) (12.7k★) | [#5976](https://github.com/livekit/agents/pull/5976) | Preserve request timeouts when callers provide custom Google HTTP options, without mutating the caller-owned options object |
| [LiveKit Agents](https://github.com/livekit/agents) (12.7k★) | [#5887](https://github.com/livekit/agents/pull/5887) | Delete trimmed empty audio items |
| [LiveKit Agents](https://github.com/livekit/agents) (12.7k★) | [#6124](https://github.com/livekit/agents/pull/6124) | Normalize two-digit years in GetDOBTask |
| [LiveKit Agents](https://github.com/livekit/agents) (12.7k★) | [#5872](https://github.com/livekit/agents/pull/5872) | Map ElevenLabs server-VAD committed transcripts to `END_OF_SPEECH`, so a realtime turn closes without a manual empty commit. |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#3924](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3924) | Reject unknown `GenerateConfig` fields up front, so a misspelled option isn't silently ignored. |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4363](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4363) | Return NaN instead of crashing when reducing an empty score list |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4167](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4167) | Route the realtime streaming sample writer through the same fallback JSON normalization as the regular log path, so sandbox objects that don't serialize cleanly can't crash an eval mid-stream |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4246](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4246) | Bound the token-count concurrency so large batches stop hammering providers at full parallelism |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4069](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4069) | Flush streamed score samples periodically, so a long eval persists score rows before it finishes. |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4267](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4267) | Keep truncate() within length when smaller than the overflow indicator |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4357](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4357) | Raise a clear error when reducing mismatched list/dict scores |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4342](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4342) | Don't cache reasoning_summaries probe failures that are transient |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4303](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4303) | Reject sample limits with more than one dash |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#3975](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3975) | Preserve call-site generation defaults when a role model override resolves, so switching a role's model doesn't drop settings like max tokens or reasoning effort. |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#3941](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3941) | Route Bedrock Nova `top_k` through the inference config instead of dropping the sampling control |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4504](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4504) | Make `registry_tag` leading parameters positional-only, so a tagged object's own keyword arguments can't collide with the decorator's |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4375](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4375) | Flatten `**kwargs` when capturing registry params so wrapped callables register cleanly |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4173](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4173) | Normalize buffer task directory URI |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4300](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4300) | Strip trailing separator in FileSystem.is_writeable |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4218](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4218) | Reuse torn checkpoint ids |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4282](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4282) | Return 0 from accuracy() on empty scores |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4090](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4090) | Clarify model-graded history prompts so `include_history=True` and final-answer placement match the actual scorer behavior |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#3982](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3982) | Preserve wrapped OpenAI reasoning payloads in the agent bridge, so encrypted provider-native reasoning survives transcript conversion. |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#3896](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3896) | Fix filestore recovery append mode: preserve carried message/tool-call pools without rehashing old segments |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#3902](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3902) | Parse OpenRouter `reasoning_details` in OpenAI-compatible responses instead of surfacing Python repr blocks |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#3895](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3895) | Honor `COLUMNS` for `TERM=dumb`: log output no longer hard-wraps at Rich's default 80 columns |
| [LMCache](https://github.com/LMCache/LMCache) (11.1k★) | [#3245](https://github.com/LMCache/LMCache/pull/3245) | Retain producer-side CUDA IPC events across MP store/retrieve so daemon IPC handles don't dereference collected events. |
| [LMCache](https://github.com/LMCache/LMCache) (11.1k★) | [#3282](https://github.com/LMCache/LMCache/pull/3282) | Handle HND GPU KV layouts in MP KV transfer, which previously mishandled that tensor format. |
| [FastMCP](https://github.com/PrefectHQ/fastmcp) (27.1k★) | [#4297](https://github.com/PrefectHQ/fastmcp/pull/4297) | Keep required discriminator tags when building tool schemas, so union arguments stay valid. |
| [FlashInfer](https://github.com/flashinfer-ai/flashinfer) (6.1k★) | [#2772](https://github.com/flashinfer-ai/flashinfer/pull/2772) | Fix compilation error: add missing `<optional>` header for `std::optional` usage in CUTLASS headers |
| [FlashInfer](https://github.com/flashinfer-ai/flashinfer) (6.1k★) | [#2756](https://github.com/flashinfer-ai/flashinfer/pull/2756) | Fix autotuner crash when input tensor is `None`: proper None-checking for optional inputs (fixes #2749) |
| [MCP Toolbox](https://github.com/googleapis/mcp-toolbox) (16.1k★) | [#3738](https://github.com/googleapis/mcp-toolbox/pull/3738) | Keep BigQuery's own error classification in execute_sql, so a 403 from an impersonated service account surfaces as a client error instead of a generic 500 |
| [MCP Toolbox](https://github.com/googleapis/mcp-toolbox) (16.1k★) | [#3516](https://github.com/googleapis/mcp-toolbox/pull/3516) | Return an error instead of panicking when a parameter type field is not a string |
| [MCP Toolbox](https://github.com/googleapis/mcp-toolbox) (16.1k★) | [#3512](https://github.com/googleapis/mcp-toolbox/pull/3512) | Report the offending value in array/map parameter type errors |
| [MCP Toolbox](https://github.com/googleapis/mcp-toolbox) (16.1k★) | [#3416](https://github.com/googleapis/mcp-toolbox/pull/3416) | Document execute_sql least-privilege setup |
| [MCP Toolbox](https://github.com/googleapis/mcp-toolbox) (16.1k★) | [#3531](https://github.com/googleapis/mcp-toolbox/pull/3531) | Validate the Looker explore_references shape instead of panicking on malformed input |
| [Pydantic AI](https://github.com/pydantic/pydantic-ai) (19.1k★) | [#5695](https://github.com/pydantic/pydantic-ai/pull/5695) | Forward penalties in completions |
| [Pydantic AI](https://github.com/pydantic/pydantic-ai) (19.1k★) | [#5694](https://github.com/pydantic/pydantic-ai/pull/5694) | Fix `MCPToolset(http_client=...)` with FastMCP by keeping `follow_redirects` out of caller-provided HTTP client factories |
| [Pydantic AI](https://github.com/pydantic/pydantic-ai) (19.1k★) | [#5474](https://github.com/pydantic/pydantic-ai/pull/5474) | Accept `providerExecuted` and `title` on Vercel AI dynamic-tool parts, so strict validation keeps the provider metadata. |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13637](https://github.com/Arize-ai/phoenix/pull/13637) | Wait for in-memory SQLite schema init before serving Phoenix, so a startup race can't hit a missing table. |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13641](https://github.com/Arize-ai/phoenix/pull/13641) | Expire prompt tool diffs on provider change, so PXI prompt editing stops carrying stale tool-change state across providers. |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13245](https://github.com/Arize-ai/phoenix/pull/13245) | Keep the generative model fetch cursor monotonic so lower-id updates cannot make later polling skip newer model changes |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13242](https://github.com/Arize-ai/phoenix/pull/13242) | Pass Anthropic computer-use beta headers for raw computer tool definitions in playground streaming and non-streaming calls |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13210](https://github.com/Arize-ai/phoenix/pull/13210) | Return NotFound-style errors for invalid GraphQL node ids instead of leaking decoder failures to clients |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13261](https://github.com/Arize-ai/phoenix/pull/13261) | Refresh span annotation notes after create so the UI shows newly added notes without a manual reload |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13533](https://github.com/Arize-ai/phoenix/pull/13533) | Clarify empty span-annotation tool input instead of failing opaquely |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13636](https://github.com/Arize-ai/phoenix/pull/13636) | Update PXI system prompt guidance to point at the current server-side Jinja templates and capability wiring instead of stale browser-side paths |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13653](https://github.com/Arize-ai/phoenix/pull/13653) | Focus the PXI input when the agent panel opens, so keyboard-first workflows start without an extra click. |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13614](https://github.com/Arize-ai/phoenix/pull/13614) | Refresh the prompts table while users stay on the page so newly created or updated prompts appear without a manual reload |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13139](https://github.com/Arize-ai/phoenix/pull/13139) | Surface playground validation errors instead of returning empty subscription payloads |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2823](https://github.com/strands-agents/harness-sdk/pull/2823) | Avoid UnboundLocalError on empty model stream |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2400](https://github.com/strands-agents/harness-sdk/pull/2400) | Support non-streaming OpenAI chat completions |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2340](https://github.com/strands-agents/harness-sdk/pull/2340) | Keep concurrent tool results in request order, so parallel execution doesn't scramble what the model sees. |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2354](https://github.com/strands-agents/harness-sdk/pull/2354) | Read vLLM `delta.reasoning` chunks in OpenAI-compatible streams so reasoning output survives provider conversion. |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2353](https://github.com/strands-agents/harness-sdk/pull/2353) | Handle Gemini safety-blocked metadata by defaulting missing usage counts and mapping safety stops to guardrail intervention |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2306](https://github.com/strands-agents/harness-sdk/pull/2306) | Normalize 3gp video format |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2304](https://github.com/strands-agents/harness-sdk/pull/2304) | Map webp images explicitly |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2656](https://github.com/strands-agents/harness-sdk/pull/2656) | Handle empty Bedrock content blocks |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2396](https://github.com/strands-agents/harness-sdk/pull/2396) | Pass structured output request params |
| [LightRAG](https://github.com/HKUDS/LightRAG) (38.6k★) | [#3206](https://github.com/HKUDS/LightRAG/pull/3206) | Honor PostgreSQL `search_path` in table-existence checks so a non-public schema is detected before migration or table creation. |
| [LightRAG](https://github.com/HKUDS/LightRAG) (38.6k★) | [#3031](https://github.com/HKUDS/LightRAG/pull/3031) | Extract Docling async markdown from the response envelope so RAG chunks carry clean document text, not JSON/base64 noise. |
| [LightRAG](https://github.com/HKUDS/LightRAG) (38.6k★) | [#2796](https://github.com/HKUDS/LightRAG/pull/2796) | Fix `None` file_path propagating as `unknown_source`: fill gaps left by #2793 |
| [LightRAG](https://github.com/HKUDS/LightRAG) (38.6k★) | [#3123](https://github.com/HKUDS/LightRAG/pull/3123) | Sync the API docs colors with the dark theme so endpoint examples stay readable in dark mode. |
| [Pipecat](https://github.com/pipecat-ai/pipecat) (14.0k★) | [#4766](https://github.com/pipecat-ai/pipecat/pull/4766) | Key cached DTMF audio by sample rate too, so the same button at a different rate stops playing back garbled |
| [Pipecat](https://github.com/pipecat-ai/pipecat) (14.0k★) | [#4553](https://github.com/pipecat-ai/pipecat/pull/4553) | Serialize interruption frames through protobuf transports so realtime voice-agent interruptions survive transport hops |
| [Graphiti](https://github.com/getzep/graphiti) (29.7k★) | [#1531](https://github.com/getzep/graphiti/pull/1531) | Strip embedded NUL bytes from FalkorDB query params, so one malformed document string can't crash a bulk graph write. |
| [Kimi Code](https://github.com/MoonshotAI/kimi-code) (6.2k★) | [#2255](https://github.com/MoonshotAI/kimi-code/pull/2255) | Customize the TUI footer status line via `status_line` config, codex / claude code style |
| [OpenHarness](https://github.com/HKUDS/OpenHarness) (15.3k★) | [#185](https://github.com/HKUDS/OpenHarness/pull/185) | TUI tab-completion: fix cursor jump, strip trailing space, accept `/quit` alias |
| [LM Evaluation Harness](https://github.com/EleutherAI/lm-evaluation-harness) (13.6k★) | [#3822](https://github.com/EleutherAI/lm-evaluation-harness/pull/3822) | Keep Anthropic stop sequences non-empty so requests are not rejected |
| [MCP Registry](https://github.com/modelcontextprotocol/registry) (7.1k★) | [#1310](https://github.com/modelcontextprotocol/registry/pull/1310) | Reject mangled publisher metadata instead of accepting malformed entries |
| [ClawTeam](https://github.com/HKUDS/ClawTeam) (5.5k★) | [#32](https://github.com/HKUDS/ClawTeam/pull/32) | Gemini CLI support: spawn, permissions, prompt injection for both backends |
| [ClawTeam](https://github.com/HKUDS/ClawTeam) (5.5k★) | [#36](https://github.com/HKUDS/ClawTeam/pull/36) | Kimi CLI support: spawn backend, permission handling, 3 new test cases |
| [ClawTeam](https://github.com/HKUDS/ClawTeam) (5.5k★) | [#40](https://github.com/HKUDS/ClawTeam/pull/40) | Pluggable TaskStore: extract task persistence into swappable backend abstraction |
| [ClawTeam](https://github.com/HKUDS/ClawTeam) (5.5k★) | [#1](https://github.com/HKUDS/ClawTeam/pull/1) | First PR: 122 tests, CI, team templates, config bugfixes, task duration tracking |
| [MCP Go SDK](https://github.com/modelcontextprotocol/go-sdk) (4.9k★) | [#962](https://github.com/modelcontextprotocol/go-sdk/pull/962) | Reject duplicate `initialize` requests so an MCP session keeps consistent protocol state after init. |
| [MCP Go SDK](https://github.com/modelcontextprotocol/go-sdk) (4.9k★) | [#981](https://github.com/modelcontextprotocol/go-sdk/pull/981) | Add `Implementation.description` metadata while keeping empty descriptions out of serialized MCP payloads |
| [Microsoft Recommenders](https://github.com/recommenders-team/recommenders) (21.9k★) | [#2345](https://github.com/recommenders-team/recommenders/pull/2345) | Query GPU memory through PyTorch first with numba as fallback, so GPU discovery doesn't fail when a CUDA context is unavailable. |
| [Microsoft Recommenders](https://github.com/recommenders-team/recommenders) (21.9k★) | [#2351](https://github.com/recommenders-team/recommenders/pull/2351) | Fail fast when TensorFlow GPU is unavailable |
| [Microsoft Recommenders](https://github.com/recommenders-team/recommenders) (21.9k★) | [#2349](https://github.com/recommenders-team/recommenders/pull/2349) | Query GPU memory with torch first |
| [Microsoft Recommenders](https://github.com/recommenders-team/recommenders) (21.9k★) | [#2322](https://github.com/recommenders-team/recommenders/pull/2322) | Honor the benchmark recommendation-count arg so eval scripts actually generate the requested top-k. |
| [Microsoft Recommenders](https://github.com/recommenders-team/recommenders) (21.9k★) | [#2350](https://github.com/recommenders-team/recommenders/pull/2350) | Label MAP@k notebook outputs consistently |
| [DB-GPT](https://github.com/eosphoros-ai/DB-GPT) (19.7k★) | [#3092](https://github.com/eosphoros-ai/DB-GPT/pull/3092) | Require explicit opt-in before the sandbox executes on the local runtime |
| [Google Gen AI SDK](https://github.com/googleapis/python-genai) (3.9k★) | [#2564](https://github.com/googleapis/python-genai/pull/2564) | Keep Live Music API keys out of websocket URLs by relying on request headers instead of duplicating secrets in query strings |
| [yfinance](https://github.com/ranaroussi/yfinance) (24.9k★) | [#2867](https://github.com/ranaroussi/yfinance/pull/2867) | Add a missing comma that was merging two equity-screener EPS fields into one |
| [EvalScope](https://github.com/modelscope/evalscope) (3.2k★) | [#1381](https://github.com/modelscope/evalscope/pull/1381) | Read SciCode assistant answers from OpenAI-style text content blocks, so the scorer prompt gets the real answer instead of an empty field. |
| [OpenHands SDK](https://github.com/OpenHands/software-agent-sdk) (971★) | [#3248](https://github.com/OpenHands/software-agent-sdk/pull/3248) | Serialize LiteLLM `modify_params` updates with an RLock so concurrent completions do not leak global parameter state |
| [OpenHands SDK](https://github.com/OpenHands/software-agent-sdk) (971★) | [#3247](https://github.com/OpenHands/software-agent-sdk/pull/3247) | Validate git workspaces with `git rev-parse --git-dir`, so a broken nested repo can't crash `/api/git/changes`. |
| [OpenHands SDK](https://github.com/OpenHands/software-agent-sdk) (971★) | [#3225](https://github.com/OpenHands/software-agent-sdk/pull/3225) | Write remote completion logs as UTF-8, so non-ASCII output survives local replay and debugging. |

### LinkedIn: https://www.linkedin.com/in/yufenghe

---

## Hi，我是何宇峰 👋

AI Agent 研究员 & 工程师 | 曾任 [Moonshot AI](https://www.moonshot.ai/) (Kimi) | 港大计算机硕士 | 上海全球AI大赛冠军 | 三次获ACM-ICPC银牌 | 曾在百度、脉脉、快手的AI 研发岗实习

- 370+ 个上游 PR 已 merged，其中 vLLM（9 个）、Mooncake（35 个）、Qwen Code（53 个）、Microsoft Agent Framework（26 个）、AstrBot（30 个）、Google ADK（10 个）、Inspect AI（22 个）、Hugging Face Transformers（1 个）、Kimi Code（1 个）、Vibe-Trading（8 个）、PyTorch（8 个）。
- 代表性公开项目（star 100+）：CoreCoder、FindJobs-Agent、RepoWiki、ContractGuard。

### 项目

| 方向 | 项目 | Stars | 简介 |
|------|------|:-----:|------|
| Coding agents / 评测 | [CoreCoder](https://github.com/he-yufeng/CoreCoder) | 1.6k+ | Claude Code 51万行源码 → 1400行 Python 核心重写，支持任意大模型，附 7 篇架构导读。 |
| 应用型 Agent | [FindJobs-Agent](https://github.com/he-yufeng/FindJobs-Agent) | 200+ | LLM 求职工具箱：技能差距分析、模拟面试、简历优化和岗位结构化。 |
| 代码库地图 | [RepoWiki](https://github.com/he-yufeng/RepoWiki) | 200+ | 开源 DeepWiki 替代品：CLI 或浏览器生成仓库 wiki，PageRank 文件排名、Mermaid 架构图、阅读指南。 |
| 应用型 Agent | [ContractGuard](https://github.com/he-yufeng/ContractGuard) | 100+ | AI 合同审查 Agent，签字前帮你找红旗条款、不公平约定和缺失保护。 |
| 代码库地图 | [GitSense](https://github.com/he-yufeng/GitSense) | 50+ | AI 开源贡献发现器 + 仓库雷达：找匹配 issue，也评估 PR 合入友好度。 |
| 代码理解 | [CodeABC](https://github.com/he-yufeng/CodeABC) | new | 面向非程序员的 AI 代码阅读器：大白话文件导读、悬浮批注、术语词典、问答、自然语言改写。 |
| Coding agents / 评测 | [AgentProbe](https://github.com/he-yufeng/AgentProbe) | new | AI Agent 回归测试 pytest 插件：快照基线、语义比较、Mock LLM。 |
| Coding agents / 评测 | [AnyCoder](https://github.com/he-yufeng/AnyCoder) | new | 终端 AI 编程 Agent，通过 litellm 支持 100+ 大模型，危险命令拦截、并行执行、会话持久化。 |
| Coding agents / 评测 | [CodeJoust](https://github.com/he-yufeng/CodeJoust) | new | AI 编程 Agent 擂台：独立 `git worktree` 运行，按测试通过率、成本、diff 大小、耗时打分。 |
| Coding agents / 评测 | [LiteBench](https://github.com/he-yufeng/LiteBench) | new | LLM / Agent benchmark 轻量 CLI + Web 面板：agent 模式、自定义 YAML、LLM judge、100+ litellm 模型。 |
| Agent 工具 | [RuleForge](https://github.com/he-yufeng/RuleForge) | new | 从代码库分析自动生成 AI 助手规则文件（CLAUDE.md、.cursorrules、copilot-instructions）。 |
| LLM 工具 | [PromptDiff](https://github.com/he-yufeng/PromptDiff) | new | LLM prompt 语义 diff：像 `git diff` 一样比较 prompt 版本。 |
| LLM 工具 | [TokenTracker](https://github.com/he-yufeng/TokenTracker) | new | 即插即用的 LLM 成本追踪：改一行 import 就能看清钱花在哪。支持 OpenAI、OpenRouter、Azure、Ollama。 |
| LLM 工具 | [BatchLLM](https://github.com/he-yufeng/BatchLLM) | new | LLM API 批处理：CSV/JSONL 进、结果出，支持并发、重试、断点续跑和成本追踪。 |
| 应用型 Agent | [IslandEscape](https://github.com/he-yufeng/IslandEscape) | new | 2D 像素风生存交易游戏：四个 LLM agent 扮演岛民，各有性格、用自然语言谈判交易、结盟博弈；和他们赛跑攒到 100 金币逃离孤岛。 |
| Agent / MCP / CI 工具 | [agentcikit](https://github.com/he-yufeng/agentcikit) | new | 一个 CLI 覆盖 AI agent、MCP 和开源贡献工作：把 CI 失败转成复现计划、给 coding agent 打包任务上下文、给 MCP server 做门禁和回放、测试工具调用安全。内含 `ci-repro`、`patch-context`、`mcp-gate`、`mcp-replay`、`tool-fence`。 |
| Coding agents / 评测 | [IssueBenchKit](https://github.com/he-yufeng/IssueBenchKit) | new | 把真实 GitHub issue 和本地 bug 打包成可复现、可评分、可分享的 coding-agent benchmark 任务。 |
| Agent 可观测性 | [FlightBox](https://github.com/he-yufeng/FlightBox) | new | AI Agent 黑盒飞行记录器：录制、脱敏、回放并 diff 本地 agent session。 |
| 量化 / 强化学习 | [DRL-MultiFactorTrading](https://github.com/he-yufeng/DRL-MultiFactorTrading) | new | 深度强化学习交易：Double DQN + Transformer attention 叠加 Fama-French 式多因子模型，含自适应风控和波动率目标。 |
| 研究 | [adversarial-refinement-imputation](https://github.com/he-yufeng/adversarial-refinement-imputation) | new | MiLeTS 2026 论文配套代码：把 R3GAN 适配到多元时间序列填补，一个范围清晰的负结果。 |
| 研究 | [TrajBias](https://github.com/he-yufeng/TrajBias) | new | 研究 LLM-as-judge 评估 agent 轨迹时的结构性偏差。 |

### 开源贡献

| 项目 | PR | 修了啥 |
|------|:--:|--------|
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5946](https://github.com/QwenLM/qwen-code/pull/5946) | 用 per-request 子 controller 隔离 Anthropic SDK 的 abort listener 泄漏，避免跨请求累积死监听器 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5020](https://github.com/QwenLM/qwen-code/pull/5020) | 取消后丢掉残留的 tool call，中止的轮次别把过期调用漏进下一次 payload。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4829](https://github.com/QwenLM/qwen-code/pull/4829) | 给 Qwen OAuth refresh 加超时，刷新端点卡住时不会把整个 CLI 挂在认证恢复上。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5071](https://github.com/QwenLM/qwen-code/pull/5071) | 流式结束后再提交已完成的快速 tool result，别让流尾的竞态把它们卡在本地队列。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#6981](https://github.com/QwenLM/qwen-code/pull/6981) | 不带 id 的流式 continuation chunk 在工具调用撞名时改为落到当前 opener 的槽位，不再进错槽 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4716](https://github.com/QwenLM/qwen-code/pull/4716) | 让 `/bug`、`/docs`、`/insight` 的浏览器打开走安全 launcher，headless 环境不再因为直接 `open` 崩。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4622](https://github.com/QwenLM/qwen-code/pull/4622) | 让 assistant 的 tool call 和它的 result 挨着，修复过的历史不再被 OpenAI 兼容 provider 拒。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5058](https://github.com/QwenLM/qwen-code/pull/5058) | 掐掉 stale 的 tool schema recall，别让 memory warning 把过期工具名带回后面的规划轮次。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#7535](https://github.com/QwenLM/qwen-code/pull/7535) | release-notes 生成的模型调用加退避重试和熔断，降级产出可见化，不再静默空窗 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5945](https://github.com/QwenLM/qwen-code/pull/5945) | 拒绝非正的 `sessionRecapAwayThresholdMinutes` 值 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5429](https://github.com/QwenLM/qwen-code/pull/5429) | 解析安装源时接受大写 URL scheme |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5426](https://github.com/QwenLM/qwen-code/pull/5426) | `mcp add` 的 transport 探测接受大写 URL scheme |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5036](https://github.com/QwenLM/qwen-code/pull/5036) | loop 检测触发后真的硬停掉重复的同一个 tool call，别让 agent 还在那反复执行卡死的动作。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4970](https://github.com/QwenLM/qwen-code/pull/4970) | 稳住截断后的 tool retry key，修复过的调用重试时身份不变，不会漂来漂去。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4673](https://github.com/QwenLM/qwen-code/pull/4673) | 修复顶层 `--list-extensions` / `-l`：按文档打印扩展列表，并在 sandbox、auth、TUI 启动前退出 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5815](https://github.com/QwenLM/qwen-code/pull/5815) | 合并 assistant 轮次时把 `reasoning_content` 丢了，多轮思维链跟着没了。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5070](https://github.com/QwenLM/qwen-code/pull/5070) | 焦点导航跳过已过期的 live agent，别让 stale 的后台 agent 行抢走键盘焦点。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4639](https://github.com/QwenLM/qwen-code/pull/4639) | 把已停用的 Qwen OAuth ACP 登录路径去掉，别再把用户导向失效的认证方式。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5752](https://github.com/QwenLM/qwen-code/pull/5752) | 把 `QWEN_SERVE_MCP_CLIENT_BUDGET` 严格按十进制整数解析 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5719](https://github.com/QwenLM/qwen-code/pull/5719) | 校验 list `maxEntries` 必须为正整数 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5679](https://github.com/QwenLM/qwen-code/pull/5679) | 严格解析 agent / workflow 的整数环境变量 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5647](https://github.com/QwenLM/qwen-code/pull/5647) | 通过 `QWEN_MODEL` 设定模型时也能识别 `USE_OPENAI` 认证 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5630](https://github.com/QwenLM/qwen-code/pull/5630) | 转义 emacs ediff 路径里的反斜杠和引号 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5494](https://github.com/QwenLM/qwen-code/pull/5494) | 空 parts 的消息不再被误当成 function call/response |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5461](https://github.com/QwenLM/qwen-code/pull/5461) | Claude 插件源接受大写 URL scheme |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5420](https://github.com/QwenLM/qwen-code/pull/5420) | 让估算的 token 拆分之和恒等于总数 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5336](https://github.com/QwenLM/qwen-code/pull/5336) | RIFF 魔数嗅探里识别 WebP 和 AVI |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5328](https://github.com/QwenLM/qwen-code/pull/5328) | 让 qwen3.6-flash 和 kimi-k2.6 预设保持纯文本 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5287](https://github.com/QwenLM/qwen-code/pull/5287) | 让四舍五入到 60s 的亚分钟时长显示为 “1m” |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5285](https://github.com/QwenLM/qwen-code/pull/5285) | 校验完整 WEBP 签名而不只是 RIFF 前缀 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5227](https://github.com/QwenLM/qwen-code/pull/5227) | 把 BMP 高度按 signed int32 读取以支持 top-down 位图 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5194](https://github.com/QwenLM/qwen-code/pull/5194) | 从正确的字节偏移读取 WebP VP8X 画布高度 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5209](https://github.com/QwenLM/qwen-code/pull/5209) | 正确读取大端 TIFF 文件里 SHORT 类型的图像尺寸 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5204](https://github.com/QwenLM/qwen-code/pull/5204) | 重开 code fence 时不再插入多余空行 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5167](https://github.com/QwenLM/qwen-code/pull/5167) | 隐藏未配置的已下线 OAuth 模型 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5073](https://github.com/QwenLM/qwen-code/pull/5073) | 上下文指令文件超预算时提前告警，别等仓库级 guidance 悄悄挤掉任务上下文。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5115](https://github.com/QwenLM/qwen-code/pull/5115) | team 功能关闭时隐藏 teammate 专属的 agent 名称参数；旧 prompt 仍传入名称时回退到 one-shot subagent，而不是直接失败 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5062](https://github.com/QwenLM/qwen-code/pull/5062) | 跨 agent 轮次带上 token escalation 上下文，delegated run 不用每轮都从容量不够的模型重来。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5077](https://github.com/QwenLM/qwen-code/pull/5077) | permission gate 拦下来时把完整计划显示出来，能看被拦的 agent 意图，而不是白白丢掉。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5061](https://github.com/QwenLM/qwen-code/pull/5061) | 保留后台 agent 的启动参数，delegated 的 CLI run 继续用你指定的执行模式。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4963](https://github.com/QwenLM/qwen-code/pull/4963) | 默认开启 fork subagent，delegated work 直接跑在隔离分支里，不用手动开。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5043](https://github.com/QwenLM/qwen-code/pull/5043) | 让 grep 结果也算通过 prior-read 检查，已经搜过的上下文不用再逼着重读一遍文件。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4828](https://github.com/QwenLM/qwen-code/pull/4828) | 认证刷新后保留用户配的共享 `baseUrl`，同模型刷新不再回退到 provider 默认 endpoint。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4715](https://github.com/QwenLM/qwen-code/pull/4715) | managed auto-memory 听运行时输出目录的，同时显式的 memory 目录覆盖仍然优先。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4596](https://github.com/QwenLM/qwen-code/pull/4596) | 爬仓库时递归进已跟踪的 Git submodule，agent 上下文才带得上子模块里的文件。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4738](https://github.com/QwenLM/qwen-code/pull/4738) | 复制可见的 CLI 输出时跳过隐藏的 thought 片段，剪贴板和屏幕上看到的一致。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4717](https://github.com/QwenLM/qwen-code/pull/4717) | 将 copy、arena、ACP snapshot 等退出路径的深拷贝改成浅层只读历史访问，同时保留 restore 写回路径的防御性克隆 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4600](https://github.com/QwenLM/qwen-code/pull/4600) | 区分 TUI 中 AUTO 与 AUTO_EDIT approval-mode 指示器：共享样式、本地化 key 和可视化证据一起补齐 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4636](https://github.com/QwenLM/qwen-code/pull/4636) | 把用户要求的输出语言也用到 side query 上，辅助回答跟主回答守同一套语言约定。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4635](https://github.com/QwenLM/qwen-code/pull/4635) | CLI todo 视图里把做完的 sticky todo 藏起来，列表只盯着还没做的。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4632](https://github.com/QwenLM/qwen-code/pull/4632) | 强化 context error 的文本抽取，嵌套的、非字符串的 payload 也能给出有用信息，而不是直接消失。 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#4607](https://github.com/QwenLM/qwen-code/pull/4607) | 修复 IDE proxy 请求：让 `fetch` 和 `EnvHttpProxyAgent` 保持在同一个 bundled `undici` 模块路径上 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (26.9k★) | [#5072](https://github.com/QwenLM/qwen-code/pull/5072) | 稳住 simple MCP 集成检查，服务就绪的时序不再让跨进程协议测试偶发挂掉。 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#1629](https://github.com/kvcache-ai/Mooncake/pull/1629) | GB200 MNNVL EP hang：`cudaMalloc` → `cuMemCreate(FABRIC)` + `cuMemMap` 跨节点 NVLink 通信 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#1644](https://github.com/kvcache-ai/Mooncake/pull/1644) | MNNVL warmup hang：跳过 fabric 连接节点的冗余握手 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2570](https://github.com/kvcache-ai/Mooncake/pull/2570) | 修复 `BatchOffload` 处理 >4 GiB 对象时的整数溢出：用 `uint64_t` 累加各 slice 大小，并拒绝超过 `uint32_t` 记录 `value_len` 的对象，而不是静默截断 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#3146](https://github.com/kvcache-ai/Mooncake/pull/3146) | 修设备选择失败路径上 UB/Barex slice 的双重释放：已入队的 slice 被塞回缓存，而所有权还在 TransferTask 手里（#3125 RDMA 修复的 sibling） |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2965](https://github.com/kvcache-ai/Mooncake/pull/2965) | `registerLocalMemory` 在后续 transport 注册失败时回滚前面已注册的 transport，避免泄漏 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#3062](https://github.com/kvcache-ai/Mooncake/pull/3062) | HA 模式下 WaitForViewChange 每次迭代都新建一个 etcd watch，改成每轮等待只建一次，堵住稳态 watch goroutine 泄漏 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#3054](https://github.com/kvcache-ai/Mooncake/pull/3054) | 恢复 wheel 多 buffer payload 的 zero-copy put，刚合入的重构把它退化成了拷贝，双提交复现后修复 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2628](https://github.com/kvcache-ai/Mooncake/pull/2628) | 修复 `CopyEnd`/`MoveEnd` 在 source 非法时的 source 引用计数泄漏 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#1831](https://github.com/kvcache-ai/Mooncake/pull/1831) | TENT NVLink IPC 修复：sub-allocated GPU tensor 使用 base pointer，将 #1622 修复移植到 TENT 路径 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#1728](https://github.com/kvcache-ai/Mooncake/pull/1728) | Hard pin 驱逐保护：模型权重永不被驱逐，const 字段 + BatchEvict 跳过 + 向后兼容序列化 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#1719](https://github.com/kvcache-ai/Mooncake/pull/1719) | 新增 `ObjectDataType` 元数据分类：KV cache、weights、tensors 等对象类型可在 metadata、snapshot 和 Python binding 中稳定传递 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2610](https://github.com/kvcache-ai/Mooncake/pull/2610) | 重构时漏掉了 `RdmaTransport::submitTransfer` 里每个 task 的 `request` 指针赋值，下游全拿到 null，status、重试、计费回读全废。追回来补上了这个关联。 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#3278](https://github.com/kvcache-ai/Mooncake/pull/3278) | 优雅关闭 watcher 线程屏蔽 SIGTERM/SIGINT：进程级信号落在 watcher 上会挂起唯一的管道读者，关闭流程永久挂死 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2311](https://github.com/kvcache-ai/Mooncake/pull/2311) | `rpc_meta` 内容没变时重复发布保持幂等，真正改了值才拒绝。 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#1825](https://github.com/kvcache-ai/Mooncake/pull/1825) | 修复 `P2PClientService::Put` 静默吞掉写入错误：传播实际错误码给调用方 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2955](https://github.com/kvcache-ai/Mooncake/pull/2955) | 无 GPU 主机跳过 CUDA 指针探测，TransferEngine 初始化不再因此失败（探测结果本就只用于打日志） |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2606](https://github.com/kvcache-ai/Mooncake/pull/2606) | 为节点内 NVLink 构建补上 `cudaStreamQuery` 映射 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2500](https://github.com/kvcache-ai/Mooncake/pull/2500) | 单 key remove 重试成功后，不再把整个 bundle cleanup 判为失败 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2651](https://github.com/kvcache-ai/Mooncake/pull/2651) | Init 遇到非数字命名的 bucket 文件时跳过，而不是直接 abort |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2629](https://github.com/kvcache-ai/Mooncake/pull/2629) | `MC_MS_AUTO_DISC` 值非法时不再中断 client 初始化 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2460](https://github.com/kvcache-ai/Mooncake/pull/2460) | 依赖安装脚本支持 EulerOS |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2927](https://github.com/kvcache-ai/Mooncake/pull/2927) | snapshot 恢复丢了 `ssd_total_capacity_bytes`，SSD 总容量在 metrics 里变 `0 B`，要等 client 重跑 `FileStorage::Init` 才恢复；把该字段随 segment 一起序列化 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2942](https://github.com/kvcache-ai/Mooncake/pull/2942) | HTTP 元数据服务器 `start()` 丢弃了 `async_start()` 的 future，bind 失败（如端口被占）在 C++ 侧完全不可见、`poll()` 永远报健康；改为检查 future 错误码 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2403](https://github.com/kvcache-ai/Mooncake/pull/2403) | 清掉失败的 io_uring sub-batch 初始化状态，别让半成品 transfer batch 把坏状态带进后续 setup。 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2402](https://github.com/kvcache-ai/Mooncake/pull/2402) | Python buddy allocator backing buffer 分配失败时直接拒绝，避免把 null raw buffer 放进 managed slab |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2962](https://github.com/kvcache-ai/Mooncake/pull/2962) | 单个 unregisterLocalMemory 改 best-effort，teardown 不再必须精确追踪注册状态 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2627](https://github.com/kvcache-ai/Mooncake/pull/2627) | 给 `UrmaContext` 析构里的 `endpoint_store_` 加空指针守卫，避免析构时崩溃 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2641](https://github.com/kvcache-ai/Mooncake/pull/2641) | 给 `MC_TCP_SLICE_SIZE` 解析裹上 `std::stoull` 异常守卫，非法值不再抛未捕获异常 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2619](https://github.com/kvcache-ai/Mooncake/pull/2619) | 修复 EFA smaps page-size 解析里 signed char 传 `isxdigit` 的 UB（#2504 的后续） |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2617](https://github.com/kvcache-ai/Mooncake/pull/2617) | 在 EFA/鲲鹏 `submitTransfer` 里补回 `task.request` 关联（与 RDMA 路径同类漏赋值） |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2602](https://github.com/kvcache-ai/Mooncake/pull/2602) | `handle_exist` 里 `is_exist` 报错时返回 HTTP 500，而不是当成“不存在” |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#2506](https://github.com/kvcache-ai/Mooncake/pull/2506) | `from_file` 里把 `enable_ssd_offload` 的字符串布尔值正确解析 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#3064](https://github.com/kvcache-ai/Mooncake/pull/3064) | 删掉 NVMe-oF 文档示例里没有任何实际作用的 `enable_mooncake_nof_pool` 配置项，别让用户照抄一个假开关 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#1626](https://github.com/kvcache-ai/Mooncake/pull/1626) | 修复非内存副本的错误日志刷屏 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (6.2k★ · 维护者) | [#3266](https://github.com/kvcache-ai/Mooncake/pull/3266) | PutStartExpiringTest 不再断言完马上检查，改成轮询等异步驱逐落位，消掉 CI 间歇性红 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#7196](https://github.com/AstrBotDevs/AstrBot/pull/7196) | 修复 Gemini thinking parts 泄漏到用户可见的消息内容中 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#6474](https://github.com/AstrBotDevs/AstrBot/pull/6474) | 修复 SQLite 并发写入 `database is locked`，添加 busy timeout |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#6596](https://github.com/AstrBotDevs/AstrBot/pull/6596) | 多模态 token 计数：图片/音频/思考链对 context 压缩不可见的问题 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#7537](https://github.com/AstrBotDevs/AstrBot/pull/7537) | 修复 Telegram media group 异常被 APScheduler 静默吞掉：try/except + EVENT_JOB_ERROR listener |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#7758](https://github.com/AstrBotDevs/AstrBot/pull/7758) | 修复 OpenAI streaming 路径复用 empty-assistant 过滤：reasoning-only 历史不再让严格 provider 返回 400 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8736](https://github.com/AstrBotDevs/AstrBot/pull/8736) | 保留 embedding API 的版本后缀，带版本的 provider endpoint 不会被归一化到错的路径。 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8750](https://github.com/AstrBotDevs/AstrBot/pull/8750) | 修好 changelog 的 anchor 链接，dashboard 的 release notes 能跳到对的小节，不再是断锚。 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8388](https://github.com/AstrBotDevs/AstrBot/pull/8388) | 补上插件详情页 sub-command 数量的 dashboard i18n，扩展详情不再露出原始翻译 key。 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8175](https://github.com/AstrBotDevs/AstrBot/pull/8175) | 修复 WeChat OA 媒体发送失败仍上报成功：prepare/send 超时或失败时向调用方抛出明确错误 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8255](https://github.com/AstrBotDevs/AstrBot/pull/8255) | 支持 RST / AsciiDoc 知识库上传：后端解析白名单和前端文件校验同步扩展，避免支持的文档格式被入口拦截 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#7398](https://github.com/AstrBotDevs/AstrBot/pull/7398) | 修复 Telegram 流式模式下空文本 sendMessageDraft 导致 400 错误刷屏 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#7217](https://github.com/AstrBotDevs/AstrBot/pull/7217) | 修复 qwen3-rerank 响应解析：兼容新旧百炼 API 格式 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8768](https://github.com/AstrBotDevs/AstrBot/pull/8768) | 清理 Lark platform id 后缀中的不可见空白，避免配置里的尾部空格破坏平台匹配 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8718](https://github.com/AstrBotDevs/AstrBot/pull/8718) | 避免多模态回复在引用文本和图片 metadata 同时存在时重复显示 quoted image caption |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8172](https://github.com/AstrBotDevs/AstrBot/pull/8172) | 优先用打包进去的 dashboard 资产，而不是过期的 data dist，发版后不再展示旧前端。 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#6710](https://github.com/AstrBotDevs/AstrBot/pull/6710) | 修复 skills-like re-query 丢失图片描述：`extra_user_content_parts` 未传递 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#6581](https://github.com/AstrBotDevs/AstrBot/pull/6581) | 修复截断器丢失唯一 user 消息导致智谱/Gemini 返回 400 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8786](https://github.com/AstrBotDevs/AstrBot/pull/8786) | 强制 persona 的工具调用边界 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8089](https://github.com/AstrBotDevs/AstrBot/pull/8089) | 图片请求在主 provider 不支持视觉输入时自动切到 vision fallback provider |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8195](https://github.com/AstrBotDevs/AstrBot/pull/8195) | 跳过空的 LLM summary，压缩时保留原始历史，不塞空占位。 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8119](https://github.com/AstrBotDevs/AstrBot/pull/8119) | 修复 active reply 图片输入丢失：把图片组件转成 image URLs 传给 LLM，保留原有文本 prompt 行为 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8061](https://github.com/AstrBotDevs/AstrBot/pull/8061) | 修复 Discord 启动同步命令触发 daily create quota 时打断 bot 启动：只把配额错误降级为 warning，其它异常继续抛出 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#8073](https://github.com/AstrBotDevs/AstrBot/pull/8073) | 修复纯图片/表情消息的知识库空 prompt：空白文本时跳过 KB 检索，避免 embedding API 400 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#7407](https://github.com/AstrBotDevs/AstrBot/pull/7407) | 修复 Gemini 原生搜索无 function tools 时 400：跳过 FunctionCallingConfig |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#7216](https://github.com/AstrBotDevs/AstrBot/pull/7216) | 修复 Gemini tool call 400：纯文本 tool result 包装为 Protobuf Struct |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#6551](https://github.com/AstrBotDevs/AstrBot/pull/6551) | 修复空 content 导致 Grok 400：content 为空时设为 None |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#7003](https://github.com/AstrBotDevs/AstrBot/pull/7003) | 修复 WebChat 长响应断连：SSE 心跳保活，context 压缩期间不再超时 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#6656](https://github.com/AstrBotDevs/AstrBot/pull/6656) | 修复 `/stop` 后新消息仍被 follow-up 捕获的竞态条件 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#6527](https://github.com/AstrBotDevs/AstrBot/pull/6527) | 修复 LLM 工具选择：重写模糊的 Upload/Download 描述 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (38.8k★) | [#6313](https://github.com/AstrBotDevs/AstrBot/pull/6313) | 修复 OpenAI API 返回 `None` choices 导致崩溃 |
| [OpenClaw](https://github.com/openclaw/openclaw) (385.5k★) | [#119127](https://github.com/openclaw/openclaw/pull/119127) | 通用 mtime 媒体清扫让出 SQLite managed 的 outgoing 子树，并在会话库不可读时 fail-closed，全域 GC 永不误删用户原件（owner P0 评审后与项目作者共建） |
| [OpenClaw](https://github.com/openclaw/openclaw) (385.5k★) | [#41271](https://github.com/openclaw/openclaw/pull/41271) | 认证配置解析失败时记录日志而非静默吞掉 |
| [OpenClaw](https://github.com/openclaw/openclaw) (385.5k★) | [#41259](https://github.com/openclaw/openclaw/pull/41259) | 目录创建失败时向上传递错误，避免 memory `ensureDir` 静默失败后继续执行 |
| [OpenClaw](https://github.com/openclaw/openclaw) (385.5k★) | [#106603](https://github.com/openclaw/openclaw/pull/106603) | sandbox-root 越界错误里改用规范的 `shortenHomePath`,报的路径和界面其余部分一致。 |
| [OpenClaw](https://github.com/openclaw/openclaw) (385.5k★) | [#96562](https://github.com/openclaw/openclaw/pull/96562) | 工具路径显示里，共享 home 前缀的同级目录不再被误缩写 |
| [OpenClaw](https://github.com/openclaw/openclaw) (385.5k★) | [#96456](https://github.com/openclaw/openclaw/pull/96456) | 按码点边界裁剪进度文本，避免落单的 surrogate |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#37884](https://github.com/vllm-project/vllm/pull/37884) | RoBERTa 的 `position_ids` 原地累积串进了 CUDA graph 的 padding，BGE-M3 跑到约 4000 请求就崩。 |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#37727](https://github.com/vllm-project/vllm/pull/37727) | Responses API 的 `instructions` 顺着 `previous_response_id` 链泄漏到了后续轮次。 |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#40789](https://github.com/vllm-project/vllm/pull/40789) | 让 V1 ubatch wrapper 认得 tuple model outputs，解开 DBO 和投机解码在 tuple 返回值上的崩溃。 |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#43243](https://github.com/vllm-project/vllm/pull/43243) | Qwen3 XML tool-call 参数先按 JSON 解析，`null`/`false` 这类 literal 在流式解析里不再被当成 Python 字面量拒掉。 |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#44821](https://github.com/vllm-project/vllm/pull/44821) | 给 DeepSeek V4 MTP projection layers 补 prefix，让 compressed-tensors 加载 draft model 时能匹配 artifact 侧 target / ignore 规则 |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#42679](https://github.com/vllm-project/vllm/pull/42679) | 保护 flash-attn rotary 导入路径，让 FA4 环境缺少 `flash_attn.ops.triton.rotary` 时稳定回退而不是构造 rotary 层时崩溃 |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#38732](https://github.com/vllm-project/vllm/pull/38732) | 修复 bench_serve 流式响应拆分多字节 UTF-8 字符导致 decode 崩溃 |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#37699](https://github.com/vllm-project/vllm/pull/37699) | 修复 weight offloading 忽略 `VLLM_WEIGHT_OFFLOADING_DISABLE_PIN_MEMORY` 环境变量 |
| [vLLM](https://github.com/vllm-project/vllm) (88.5k★) | [#37301](https://github.com/vllm-project/vllm/pull/37301) | 修复 base64 JPEG 视频帧返回空 metadata：补充帧数、fps、时长 |
| [PyTorch](https://github.com/pytorch/pytorch) (102.3k★) | [#188229](https://github.com/pytorch/pytorch/pull/188229) | `avg_pool3d` backward 在超过 `INT_MAX` 元素的输入上静默算错梯度：atomic scatter kernel 用 32 位 `int` 算偏移和边界，改成 64 位索引（PR 显示 Closed，经 pytorchmergebot 合入） |
| [PyTorch](https://github.com/pytorch/pytorch) (102.3k★) | [#188022](https://github.com/pytorch/pytorch/pull/188022) | 让 CuTeDSL 的 topk override 守住非当前 CUDA 设备，避免把工作分发到错误设备（PR 显示 Closed，经 pytorchmergebot 合入） |
| [PyTorch](https://github.com/pytorch/pytorch) (102.3k★) | [#186779](https://github.com/pytorch/pytorch/pull/186779) | 不支持的 batch norm 三阶导改为显式报错，不再静默返回错误梯度（PR 显示 Closed，经 pytorchmergebot 合入） |
| [PyTorch](https://github.com/pytorch/pytorch) (102.3k★) | [#188027](https://github.com/pytorch/pytorch/pull/188027) | 在 Laguerre / Legendre 多项式的辅助函数里初始化 `r`，避免边界路径返回未初始化内存（PR 显示 Closed，经 pytorchmergebot 合入） |
| [PyTorch](https://github.com/pytorch/pytorch) (102.3k★) | [#187860](https://github.com/pytorch/pytorch/pull/187860) | 把 `meta__transformer_encoder_layer_fwd` 里对空 `src` 的检查改走 `guard_or_false`，让 `torch.compile` 下 unbacked 符号 `numel` 不再抛数据依赖错误（PR 显示 Closed，经 pytorchmergebot 合入） |
| [PyTorch](https://github.com/pytorch/pytorch) (102.3k★) | [#176100](https://github.com/pytorch/pytorch/pull/176100) | 修复 Inductor codegen 中用户自定义 Triton kernel 的名称修饰，避免不同 kernel 在生成代码里命名冲突（PR 显示 Closed，经 pytorchmergebot 合入） |
| [PyTorch](https://github.com/pytorch/pytorch) (102.3k★) | [#187643](https://github.com/pytorch/pytorch/pull/187643) | 修复 `stale_issues` workflow 的 `parse_older_than` 在非闰年崩溃：朴素的 2 月 29 日偏移会抛 `ValueError`（PR 显示 Closed，经 pytorchmergebot 合入） |
| [PyTorch](https://github.com/pytorch/pytorch) (102.3k★) | [#187262](https://github.com/pytorch/pytorch/pull/187262) | 移除过时的 `setuptools` 版本上限，让构建解析到当前工具链而不是被钉在旧版本（PR 显示 Closed，经 pytorchmergebot 合入） |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#3797](https://github.com/bytedance/deer-flow/pull/3797) | 同步 MCP session-pool 单例生命周期,避免并发首次使用创建重复池 |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#3799](https://github.com/bytedance/deer-flow/pull/3799) | 串行化单个聊天的线程创建，并发消息不再给一个聊天建出重复线程。 |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#3800](https://github.com/bytedance/deer-flow/pull/3800) | 让 `create_thread` 在并发 insert 输掉竞争时保持幂等，避免一个聊天产生重复 thread。 |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#4157](https://github.com/bytedance/deer-flow/pull/4157) | subagent 的 `description` 是 agent 可编辑的(setup_agent / update_agent),却原样渲染进 `<subagent_system>` 块,构造的首行能越界伪造框架标签。转义掉,和 `<soul>` 那个修复同类。 |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#4137](https://github.com/bytedance/deer-flow/pull/4137) | 在 `SOUL.md` 进入 `<soul>` system-prompt 块前 HTML 转义,让可被 agent 编辑的 personality 无法伪造框架标签、越出信任边界 |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#3778](https://github.com/bytedance/deer-flow/pull/3778) | 同步 skill storage 单例的生命周期 |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#3631](https://github.com/bytedance/deer-flow/pull/3631) | 从 streamed values 事件里剥离 base64 图片数据 |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#4216](https://github.com/bytedance/deer-flow/pull/4216) | `get_memory_config()` 只作为 `get_app_config()` 的副作用刷新，agent factory 这类直接读者在 config.yaml 改完后拿到旧的 `memory.mode`；改走 `get_app_config()` 并加 FileNotFoundError 兜底 |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#4429](https://github.com/bytedance/deer-flow/pull/4429) | fork 恢复的检查点把 sandbox channel 以 langgraph `Overwrite` 包装态送达，sync/async 初始化路径和 sibling readers 统一走一个解包 helper |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#4381](https://github.com/bytedance/deer-flow/pull/4381) | after_agent 钩子里的 sandbox state 被 Overwrite 包了一层，解包后再消费，不再取不到值 |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#4253](https://github.com/bytedance/deer-flow/pull/4253) | 工具结果里字面的 `</tool_response>` 能提前闭合 MindIE framing、注入尾随文本;转义 tool-response 内容,和同函数里 tool-call name/arg 的转义保持一致。 |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#4130](https://github.com/bytedance/deer-flow/pull/4130) | 把 requests/httpx 剩余 HTTP 方法也识别为网络 sink |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#3674](https://github.com/bytedance/deer-flow/pull/3674) | 让 UI 运行时 channel 配置优先于 config.yaml |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#3719](https://github.com/bytedance/deer-flow/pull/3719) | `_apply_updates` 跳过纯空白 facts,避免空白记忆条目堆积 |
| [deer-flow](https://github.com/bytedance/deer-flow) (79.6k★) | [#3709](https://github.com/bytedance/deer-flow/pull/3709) | 修复同内容 todo 列表耗尽后 positional fallback 误吞不相关 todo |
| [Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) (30.3k★ · 维护者) | [#777](https://github.com/HKUDS/Vibe-Trading/pull/777) | Portfolio Studio 首刀「组合风险透视」：纯计算核心（集中度/波动/回撤/VaR/分散度/相关性）加走 loader fallback 链取数的 agent 工具 |
| [Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) (30.3k★ · 维护者) | [#900](https://github.com/HKUDS/Vibe-Trading/pull/900) | 每次回测都会产出 risk x-ray 工件（JSON + Markdown），基于策略的平均持仓计算集中度、波动、回撤和尾部风险，并汇入 run 指标 |
| [Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) (30.3k★ · 维护者) | [#818](https://github.com/HKUDS/Vibe-Trading/pull/818) | Portfolio Studio 第二步：可组合的组合权重约束，能挂到任意优化器上，waterfill 再分配只喂给还没到上限的仓位 |
| [Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) (30.3k★ · 维护者) | [#796](https://github.com/HKUDS/Vibe-Trading/pull/796) | 把 strict bench 门禁接进 CLI：`alpha bench --strict` 在策略不达标时直接判失败 |
| [Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) (30.3k★ · 维护者) | [#795](https://github.com/HKUDS/Vibe-Trading/pull/795) | Portfolio Studio 的 rebalance notes：回测器每次调仓产出带指标的 notes 工件，agent 驱动的调仓可审计回看 |
| [Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) (30.3k★ · 维护者) | [#966](https://github.com/HKUDS/Vibe-Trading/pull/966) | 在 run 详情页直接展示 Portfolio Studio 产物（risk x-ray、调仓 notes），跑完即看不用翻文件 |
| [Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) (30.3k★ · 维护者) | [#970](https://github.com/HKUDS/Vibe-Trading/pull/970) | yfinance 数据源的加密货币回测改走 CryptoEngine，BTC/ETH 这类标的不再报错 |
| [Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) (30.3k★ · 维护者) | [#984](https://github.com/HKUDS/Vibe-Trading/pull/984) | 层级路由写入的记忆条目补上 .md 扩展名，修复写入即隐形（裸 slug 文件对所有发现路径不可见） |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5808](https://github.com/microsoft/agent-framework/pull/5808) | handoff 原地改了 message 的 role，重试复用时把改动泄漏出去了，改成复用消毒过的副本。 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5462](https://github.com/microsoft/agent-framework/pull/5462) | 修复 `background=True` + tools 无限 retrieve loop：清掉已完成的 continuation 状态，让 tool results 正常提交 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5773](https://github.com/microsoft/agent-framework/pull/5773) | 把同步的 Python 工具挪出事件循环跑，阻塞型调用不再冻住并发的 agent 任务。 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5815](https://github.com/microsoft/agent-framework/pull/5815) | 把 MCP `tools/list` 的元数据转发到 `call_tool` instrumentation，trace 里的工具注解不丢。 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5801](https://github.com/microsoft/agent-framework/pull/5801) | 按 call id 合并 code interpreter 的流式历史片段，存下来的代码和结果完整，也不会重复记 delta。 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#7162](https://github.com/microsoft/agent-framework/pull/7162) | Python：Anthropic 流式把 token 用量数了两遍，流式增量之上又累加了最终消息用量 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#6132](https://github.com/microsoft/agent-framework/pull/6132) | 按 session id 过滤 filesystem checkpoint index，重开 store 不再返回别的 workflow session 的 checkpoint。 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5904](https://github.com/microsoft/agent-framework/pull/5904) | AG-UI thread id 下继续用 ChatClientAgent 的本地历史 provider，别把 session 历史当成服务端托管的模型历史。 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5976](https://github.com/microsoft/agent-framework/pull/5976) | 修复 sequential workflow 示例输出，让非 streaming 结果展示所有参与 agent 的回复 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5799](https://github.com/microsoft/agent-framework/pull/5799) | 补齐 Handoff workflow 的 name/description 元数据传递，让 builder 和 hosting 注册都能命名工作流 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#7256](https://github.com/microsoft/agent-framework/pull/7256) | Python：`from_dict` 拿 payload 自己声明的 type 校验它自己，恒真等于没校验；改成从类解析应有类型 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#7108](https://github.com/microsoft/agent-framework/pull/7108) | Python：`FunctionTool.invoke` 用 `exclude_none=True` 导出参数，模型有意给必需可空参数传的 `null` 被丢掉，调用直接缺参失败；改用 `exclude_unset` 保留显式 null |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#6210](https://github.com/microsoft/agent-framework/pull/6210) | reasoning payload 被剥掉时一并丢掉 hosted MCP 的 tool-call 历史，stateless 的 OpenAI replay 不再发孤立的 MCP 调用。 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5861](https://github.com/microsoft/agent-framework/pull/5861) | Foundry handoff 的结构化参数在 response 转换里丢了，delegated agent 调用跟着废，改成保留原结构。 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#7239](https://github.com/microsoft/agent-framework/pull/7239) | Python：AG-UI MESSAGES_SNAPSHOT 的消息顺序与模型原始产出顺序不一致，改为保持发射顺序 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#7130](https://github.com/microsoft/agent-framework/pull/7130) | Python：topic selection 的关键词提取支持非英文文本，中文、日文等非拉丁查询不再空手而归 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#7124](https://github.com/microsoft/agent-framework/pull/7124) | Python：compaction 估 token 时用 `ensure_ascii=True` 序列化消息，tokenizer 数的是 `\uXXXX` 转义序列而不是真实字符（CJK 约虚高 1.6 倍）；改成按真实文本序列化 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#6640](https://github.com/microsoft/agent-framework/pull/6640) | Python：为 Bedrock 和 Gemini connector 暴露 cache 与 reasoning token 计数 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#6491](https://github.com/microsoft/agent-framework/pull/6491) | .NET：修复 fan-in barrier 的 checkpoint 状态 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#6208](https://github.com/microsoft/agent-framework/pull/6208) | 声明式 `Foreach` 把多字段的 PowerFx table row 折叠了，改成整行 record 值原样带过每次迭代。 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5784](https://github.com/microsoft/agent-framework/pull/5784) | 转换历史时跳过孤立的 Anthropic thinking signature，replay 不再带上无效的独立签名。 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#6040](https://github.com/microsoft/agent-framework/pull/6040) | 把 Foundry agent 的 `default_headers` 透传到 OpenAI client 创建，自定义的认证、路由 header 在初始化后还在。 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#6037](https://github.com/microsoft/agent-framework/pull/6037) | 保留 Foundry citation `get_url` 元数据，让检索引用链接经过 response conversion 后仍能出现在 chat response 中 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5974](https://github.com/microsoft/agent-framework/pull/5974) | 让 Foundry agent eval 映射保留工具定义，评测运行能正常调用代码定义的 tools |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5800](https://github.com/microsoft/agent-framework/pull/5800) | 修复 AG-UI tool result message id 冲突：provider 省略 update id 时仍能生成独立 fallback id |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (12.7k★) | [#5778](https://github.com/microsoft/agent-framework/pull/5778) | 补上 Magentic protocol 的消息声明，orchestrator 的 chat/reset 信号能反序列化，不再卡在未知类型上。 |
| [opencode](https://github.com/anomalyco/opencode) (195.0k★) | [#30022](https://github.com/anomalyco/opencode/pull/30022) | 把 MCP OAuth 回调服务绑到 IPv4 loopback，让浏览器回跳稳定连上、不再和 IPv6 抢地址 |
| [dify](https://github.com/langgenius/dify) (151.8k★) | [#39953](https://github.com/langgenius/dify/pull/39953) | 给没有超时的 TiDB Cloud API 调用补上有界超时，集群端点挂起不再无限拖住 vdb 操作 |
| [dify](https://github.com/langgenius/dify) (151.8k★) | [#37425](https://github.com/langgenius/dify/pull/37425) | 给 OperationService 计费请求加超时，慢计费端点挂不住请求。 |
| [dify](https://github.com/langgenius/dify) (151.8k★) | [#39479](https://github.com/langgenius/dify/pull/39479) | 邮件限流的 IP 首击窗口真正生效：GET 判空再 SETEX 的竞态改为 SET NX 原子认领 |
| [dify](https://github.com/langgenius/dify) (151.8k★) | [#38801](https://github.com/langgenius/dify/pull/38801) | 在 service-api 和 explore 端点提前校验 conversation，坏的 `conversation_id` 直接 404，而不是流式跑到后期才失败。 |
| [dify](https://github.com/langgenius/dify) (151.8k★) | [#37685](https://github.com/langgenius/dify/pull/37685) | watercrawl 请求超时保持有界,而不是用 `timeout=None` 禁用 |
| [dify](https://github.com/langgenius/dify) (151.8k★) | [#37669](https://github.com/langgenius/dify/pull/37669) | legacy dataset 配置提取时跳过空的 tool entry |
| [Transformers](https://github.com/huggingface/transformers) (163.5k★) | [#44710](https://github.com/huggingface/transformers/pull/44710) | `AutoProcessor.from_pretrained` 静默丢掉了 `revision`、`token` 这些 hub kwargs。 |
| [OpenHands](https://github.com/OpenHands/OpenHands) (83.5k★) | [#14776](https://github.com/OpenHands/OpenHands/pull/14776) | 编辑 basic model 设置时保留自定义的 LLM base URL，存下来的 profile 不再静默回退到 provider 默认 endpoint。 |
| [Firecrawl](https://github.com/firecrawl/firecrawl) (163.2k★) | [#3730](https://github.com/firecrawl/firecrawl/pull/3730) | self-host 抓取的 interact 动作明确报错拒绝，而不是隐晦地失败 |
| [Firecrawl](https://github.com/firecrawl/firecrawl) (163.2k★) | [#3729](https://github.com/firecrawl/firecrawl/pull/3729) | self-host bypass 路径保留 auth chunk，已认证的 self-host 抓取不再被丢掉。 |
| [Firecrawl](https://github.com/firecrawl/firecrawl) (163.2k★) | [#3713](https://github.com/firecrawl/firecrawl/pull/3713) | Python SDK 正确处理 async v1 batch scrape 以 dict 形式返回的响应 |
| [SGLang](https://github.com/sgl-project/sglang) (31.5k★) | [#20739](https://github.com/sgl-project/sglang/pull/20739) | 修复 hybrid_linear_attn_backend 与 ngram 投机采样同时使用时崩溃 |
| [SGLang](https://github.com/sgl-project/sglang) (31.5k★) | [#21472](https://github.com/sgl-project/sglang/pull/21472) | 修复 `--backend diffusers` 在非 T2I 模型上的 `PicklingError` |
| [DeepSpeed](https://github.com/deepspeedai/DeepSpeed) (42.9k★) | [#8049](https://github.com/deepspeedai/DeepSpeed/pull/8049) | eigenvalue monitor 的值算了却没写日志，接上后才真正落进记录。 |
| [Triton](https://github.com/triton-lang/triton) (19.9k★) | [#10883](https://github.com/triton-lang/triton/pull/10883) | 除法和取模先把 fp8 操作数提升精度再算，不再直接按 fp8 精度求值（BC breaking） |
| [Triton](https://github.com/triton-lang/triton) (19.9k★) | [#10689](https://github.com/triton-lang/triton/pull/10689) | 分数 `top_k` 向下取整为 0 时至少保留一个 config |
| [Triton](https://github.com/triton-lang/triton) (19.9k★) | [#10687](https://github.com/triton-lang/triton/pull/10687) | `is_power_of_two(0)` 误返回了 True。 |
| [Triton](https://github.com/triton-lang/triton) (19.9k★) | [#9613](https://github.com/triton-lang/triton/pull/9613) | 修复 AxisInfo 正确性：有符号常量、未知 shift 和 shift UB 都保守处理 |
| [Cline](https://github.com/cline/cline) (65.9k★) | [#11166](https://github.com/cline/cline/pull/11166) | open-tabs 的 host RPC 挂了也能搜文件，回退到系统 `rg`，不让搜索整个失效。 |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1822](https://github.com/agentscope-ai/agentscope/pull/1822) | 给内置 Bash tool 增加 cwd 选项，让 shell 命令能在指定 workspace 目录执行 |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1823](https://github.com/agentscope-ai/agentscope/pull/1823) | 把 workspace root 加进 permission context，chat run 按 agent 真正能看到的 workspace 去授权文件。 |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1815](https://github.com/agentscope-ai/agentscope/pull/1815) | team run 里继承 leader 的权限规则，delegated agent 守着和 leader 一样的 workspace、文件访问约束。 |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1734](https://github.com/agentscope-ai/agentscope/pull/1734) | append 和 streaming replace 时刷新 Redis message list 的 TTL，配置的存储 TTL 才真正约束聊天历史。 |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1786](https://github.com/agentscope-ai/agentscope/pull/1786) | 创建 Redis session 时保留调用方给的 id，后面的 get/update/list 命中同一个 session，而不是新生成的 UUID。 |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1717](https://github.com/agentscope-ai/agentscope/pull/1717) | Windows 上启动 Bash tool 子进程时使用 `CREATE_NO_WINDOW`，避免工具执行弹出控制台窗口 |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1883](https://github.com/agentscope-ai/agentscope/pull/1883) | 处理没有 id 的 Gemini function call |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1774](https://github.com/agentscope-ai/agentscope/pull/1774) | 显式设置 Qwen `thinking_enable` 时转发到 OpenAI-compatible `extra_body`，同时不污染普通 OpenAI 请求 |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (28.7k★) | [#1732](https://github.com/agentscope-ai/agentscope/pull/1732) | 汇总所有启用的 tool group 的 skill，prompt instructions 和 Skill viewer 跟当前启用的工具对得上。 |
| [LiteLLM](https://github.com/BerriAI/litellm) (55.9k★) | [#26401](https://github.com/BerriAI/litellm/pull/26401) | 修复 `LITELLM_LOG=INFO` 漏设 `verbose_logger`：proxy INFO 日志不再静默丢失 |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#10089](https://github.com/promptfoo/promptfoo/pull/10089) | trace-span-duration 越界百分位直接拒绝，不再静默算出无意义结果 |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9850](https://github.com/promptfoo/promptfoo/pull/9850) | 空 token 输入的 GLEU 评分返回 0 分，不再报错 |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#10124](https://github.com/promptfoo/promptfoo/pull/10124) | Azure provider 空 completion `choices` 数组不再崩溃 |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#10076](https://github.com/promptfoo/promptfoo/pull/10076) | 工具调用缺 `function` 对象时 tool-call 断言抛 TypeError;改成返回 `pass:false`。 |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9867](https://github.com/promptfoo/promptfoo/pull/9867) | 读取 Azure logprobs 时空 `choices` 数组不再崩溃 |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9897](https://github.com/promptfoo/promptfoo/pull/9897) | 给 Bedrock Titan 和 Cohere provider 的数组访问加守卫，空响应数组不再让生成崩掉。 |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9815](https://github.com/promptfoo/promptfoo/pull/9815) | 拒绝畸形的 `__expected0` CSV 表头,而不是静默丢弃它的断言 |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9824](https://github.com/promptfoo/promptfoo/pull/9824) | 修正 inverse JSON 断言的失败信息，不再把方向写反 |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9841](https://github.com/promptfoo/promptfoo/pull/9841) | 空输出返回 `pass:false` 而不是抛异常 |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9840](https://github.com/promptfoo/promptfoo/pull/9840) | 保留 JSONL 行的 description 而不是覆盖 |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9761](https://github.com/promptfoo/promptfoo/pull/9761) | contains-any/all 断言值里保留引号内的逗号 |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9822](https://github.com/promptfoo/promptfoo/pull/9822) | `maxLen` 小于 3 时 ellipsize 仍不超过 maxLen |
| [promptfoo](https://github.com/promptfoo/promptfoo) (24.1k★) | [#9757](https://github.com/promptfoo/promptfoo/pull/9757) | array metadata 值里所有转义逗号都还原 |
| [goose](https://github.com/aaif-goose/goose) (52.6k★) | [#9528](https://github.com/aaif-goose/goose/pull/9528) | 恢复 desktop 应用里 new chat 快捷键的导航 |
| [goose](https://github.com/aaif-goose/goose) (52.6k★) | [#9599](https://github.com/aaif-goose/goose/pull/9599) | 改用阻塞式的 OTLP HTTP exporter，进程退出时遥测数据不丢。 |
| [goose](https://github.com/aaif-goose/goose) (52.6k★) | [#9584](https://github.com/aaif-goose/goose/pull/9584) | 显示 skill 支持文件解析后的真实路径，而不是未解析的占位符 |
| [GitHub MCP Server](https://github.com/github/github-mcp-server) (32.1k★) | [#2514](https://github.com/github/github-mcp-server/pull/2514) | PR review 请求支持 team reviewer，把 team slug 解析成 GitHub review subject，而不是直接丢掉。 |
| [GitHub MCP Server](https://github.com/github/github-mcp-server) (32.1k★) | [#2612](https://github.com/github/github-mcp-server/pull/2612) | read-only 模式下隐藏会写入 GitHub 的 UI resources，同时保留安全的只读资源注册 |
| [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) (28.5k★) | [#3643](https://github.com/openai/openai-agents-python/pull/3643) | 上报实际生效的 Blaxel 超时值，而不是未配置的默认值 |
| [ms-swift](https://github.com/modelscope/ms-swift) (15.1k★) | [#9642](https://github.com/modelscope/ms-swift/pull/9642) | DPO 数据准备阶段遇到空 `rejected_messages` 直接快速失败，不用等训练跑到一半才崩。 |
| [ms-swift](https://github.com/modelscope/ms-swift) (15.1k★) | [#9816](https://github.com/modelscope/ms-swift/pull/9816) | `--torch_dtype` 失效期间用户只能靠 engine_kwargs 传 dtype，flag 修好后两边撞参数直接 TypeError；splat 前 pop 掉并让 flag 恒赢 |
| [ms-swift](https://github.com/modelscope/ms-swift) (15.1k★) | [#9750](https://github.com/modelscope/ms-swift/pull/9750) | 视频元数据损坏时 `get_avg_fps()` 返回 0，`range(0, len(vr), 0)` 在读到第一帧前就抛 ValueError；给 MiniCPM-V / mPLUG-Owl3 的采样步长加守卫 |
| [ms-swift](https://github.com/modelscope/ms-swift) (15.1k★) | [#9605](https://github.com/modelscope/ms-swift/pull/9605) | 不同格式的图片在临时缓存里撞了键，把 mode 和 size 也纳入 key 才分开。 |
| [ms-swift](https://github.com/modelscope/ms-swift) (15.1k★) | [#9612](https://github.com/modelscope/ms-swift/pull/9612) | `_replace_system` 把非字符串的 prefix 元素压平了，模板化 system prompt 的结构化内容被抹掉。 |
| [ms-swift](https://github.com/modelscope/ms-swift) (15.1k★) | [#9789](https://github.com/modelscope/ms-swift/pull/9789) | CUDA 测试容器里升级老 wandb，其旧 pb2 与 protobuf 7.x 相冲曾致全仓 CI 红 |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1735](https://github.com/ag-ui-protocol/ag-ui/pull/1735) | 修复 HITL tool call 后 ADK session 可能被旧状态回写的问题 |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1890](https://github.com/ag-ui-protocol/ag-ui/pull/1890) | 在一次 ADK execution 内缓存 session 读取，远端 session service 不用在每次 agent 运行前重复拉一遍。 |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1828](https://github.com/ag-ui-protocol/ag-ui/pull/1828) | 识别 Strands 私有的 session manager，AG-UI 回放历史时尊重活跃 session，不再重播旧轮次。 |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1889](https://github.com/ag-ui-protocol/ag-ui/pull/1889) | 构建 ADK workflow graph 时把 output_schema 的 agent 也收进来，结构化输出的节点不再漏。 |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1848](https://github.com/ag-ui-protocol/ag-ui/pull/1848) | 打包回放的 tool results |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1730](https://github.com/ag-ui-protocol/ag-ui/pull/1730) | 允许 CopilotKit 1.x 的 runtime peer 依赖 |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1826](https://github.com/ag-ui-protocol/ag-ui/pull/1826) | 把 LangGraph 的 runtime context 透传进 tool kwargs，graph tool 保住调用方传的执行上下文。 |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1832](https://github.com/ag-ui-protocol/ag-ui/pull/1832) | LangGraph 转换文本和媒体 block 时保留 AG-UI `InputContent.metadata` |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1829](https://github.com/ag-ui-protocol/ag-ui/pull/1829) | LangGraph 流从文本切到 tool call 时先关闭当前文本消息，避免工具调用事件被前一段文本吞掉 |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (15.2k★) | [#1769](https://github.com/ag-ui-protocol/ag-ui/pull/1769) | 将 proto generation 从 Unix-only `mkdir -p` 改为跨平台 Node 脚本，兼容 Windows `.CMD` plugin shim |
| [cherry-studio](https://github.com/CherryHQ/cherry-studio) (50.1k★) | [#16352](https://github.com/CherryHQ/cherry-studio/pull/16352) | 在截断边界保住 surrogate pair，多字节字符不会被切成半个非法字符。 |
| [cherry-studio](https://github.com/CherryHQ/cherry-studio) (50.1k★) | [#17106](https://github.com/CherryHQ/cherry-studio/pull/17106) | 估算 API 网关 token 用量时把嵌套在 `tool_result` 里的图片计入，多模态工具结果不再被少算 |
| [cherry-studio](https://github.com/CherryHQ/cherry-studio) (50.1k★) | [#16358](https://github.com/CherryHQ/cherry-studio/pull/16358) | aihubmix 路径丢弃 Ideogram 里没有可用 URL 的 `data[]` 项,不再渲染坏图 |
| [cherry-studio](https://github.com/CherryHQ/cherry-studio) (50.1k★) | [#16454](https://github.com/CherryHQ/cherry-studio/pull/16454) | 保留 citations 里的纯 URL markdown 引用行,不再丢弃 |
| [cherry-studio](https://github.com/CherryHQ/cherry-studio) (50.1k★) | [#16361](https://github.com/CherryHQ/cherry-studio/pull/16361) | 为大写扩展名正确解析 `.d.ts` 图标 |
| [cherry-studio](https://github.com/CherryHQ/cherry-studio) (50.1k★) | [#16217](https://github.com/CherryHQ/cherry-studio/pull/16217) | 相对时间在单位边界正确进位 |
| [Google ADK](https://github.com/google/adk-python) (21.0k★) | [#5698](https://github.com/google/adk-python/pull/5698) | 让 `final_response_match_v2` 在 criterion 选择开启时把 intermediate responses 纳入最终回答评判 |
| [Mem0](https://github.com/mem0ai/mem0) (62.8k★) | [#5380](https://github.com/mem0ai/mem0/pull/5380) | 暴露 Qdrant 的 `https` 选项，自托管的 HTTP 集群用 API key 认证就行，不用被逼进 TLS client 模式。 |
| [Mem0](https://github.com/mem0ai/mem0) (62.8k★) | [#5416](https://github.com/mem0ai/mem0/pull/5416) | 修复 S3 Vectors entity index 命名，避免 agent memory 写入因 AWS index-name 校验失败 |
| [Mem0](https://github.com/mem0ai/mem0) (62.8k★) | [#5383](https://github.com/mem0ai/mem0/pull/5383) | OpenClaw CLI metadata 注册时跳过 runtime setup，插件发现阶段不再重复注册运行时副作用。 |
| [verl](https://github.com/verl-project/verl) (22.9k★) | [#6620](https://github.com/verl-project/verl/pull/6620) | 按 DP 和 TP rank 算 colocated vLLM 权重同步的 ZMQ socket rank，多个 DP worker 不再挤到同一个 receiver。 |
| [TRL](https://github.com/huggingface/trl) (19.0k★) | [#6054](https://github.com/huggingface/trl/pull/6054) | SFT 准备阶段遇到已经转换过的数据集直接报错，别静默产出错的训练 batch。 |
| [TRL](https://github.com/huggingface/trl) (19.0k★) | [#6063](https://github.com/huggingface/trl/pull/6063) | 保留 vLLM prompt 的 special tokens |
| [Agno](https://github.com/agno-agi/agno) (41.6k★) | [#8131](https://github.com/agno-agi/agno/pull/8131) | 保留非哨兵工具参数字符串里的空白，同时继续只对精确的 None / True / False 哨兵做归一化 |
| [RAGFlow](https://github.com/infiniflow/ragflow) (87.1k★) | [#15691](https://github.com/infiniflow/ragflow/pull/15691) | 跳过空的 agent switch 条件，空分支判断不会让有效的后续 agent 流程崩掉或卡住。 |
| [RAGFlow](https://github.com/infiniflow/ragflow) (87.1k★) | [#15696](https://github.com/infiniflow/ragflow/pull/15696) | 重复的 n-hop GraphRAG 边保留最强的 PageRank 分，路径顺序覆盖不了排序。 |
| [RAGFlow](https://github.com/infiniflow/ragflow) (87.1k★) | [#15601](https://github.com/infiniflow/ragflow/pull/15601) | Docling native 解析没产出 chunk 时降级，文档还能出可用内容，而不是空解析。 |
| [LiveKit Agents](https://github.com/livekit/agents) (12.7k★) | [#5864](https://github.com/livekit/agents/pull/5864) | 暴露 Soniox STT server error：流式识别失败时返回明确错误，不再被当成空 transcript |
| [LiveKit Agents](https://github.com/livekit/agents) (12.7k★) | [#5820](https://github.com/livekit/agents/pull/5820) | 修复 Anthropic streaming retry：瞬时建流失败后重新创建 stream，不再重复 await 同一个 coroutine |
| [LiveKit Agents](https://github.com/livekit/agents) (12.7k★) | [#5994](https://github.com/livekit/agents/pull/5994) | 兼容 OpenAI 兼容 realtime 返回字符串的 status details，incomplete response 不再在日志路径崩。 |
| [LiveKit Agents](https://github.com/livekit/agents) (12.7k★) | [#5976](https://github.com/livekit/agents/pull/5976) | 调用方传入自定义 Google HTTP options 时仍保留请求 timeout，并避免原地修改调用方对象 |
| [LiveKit Agents](https://github.com/livekit/agents) (12.7k★) | [#5887](https://github.com/livekit/agents/pull/5887) | 删除裁剪后为空的 audio item |
| [LiveKit Agents](https://github.com/livekit/agents) (12.7k★) | [#6124](https://github.com/livekit/agents/pull/6124) | `GetDOBTask` 里规范化两位数年份 |
| [LiveKit Agents](https://github.com/livekit/agents) (12.7k★) | [#5872](https://github.com/livekit/agents/pull/5872) | 把 ElevenLabs server-VAD 的 committed transcript 映射成 `END_OF_SPEECH`，realtime turn 不用手动空 commit 才结束。 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#3924](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3924) | 未知的 `GenerateConfig` 字段提前报错，拼错的生成参数不再被静默忽略。 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4363](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4363) | reduce 空 score 列表时返回 NaN 而不是崩溃 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4167](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4167) | 让实时流式 sample 写出走与常规日志路径相同的 fallback JSON 归一化，无法序列化的 sandbox 对象不再让评测中途崩掉。 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4246](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4246) | token 计数并发加上限，大批量不再全并发打满 provider |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4069](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4069) | 周期性 flush 流式 score sample，长时间评测在结束前也能持续把 score 落盘。 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4267](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4267) | `truncate()` 在长度小于溢出指示符时仍保持在限制内 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4357](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4357) | reduce 不匹配的 list/dict scores 时抛出清晰错误 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4342](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4342) | 不缓存瞬时的 reasoning_summaries 探测失败 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4303](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4303) | 拒绝含多个连字符的 sample limit |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#3975](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3975) | 解析 role model override 时保留调用侧的生成默认值，角色换模型不会丢掉 max tokens、reasoning effort 这些设置。 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#3941](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3941) | 修复 Bedrock Nova `top_k` 路由：把采样控制传到 inference config，而不是被静默丢弃 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4504](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4504) | `registry_tag` 的前置参数改为仅位置传参，被标记对象自己的同名关键字参数不再撞上装饰器参数 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4375](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4375) | registry 捕获参数时把 **kwargs 拍平，包装过的可调用对象注册不再出错 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4173](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4173) | 规范化 buffer task 目录 URI |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4300](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4300) | `FileSystem.is_writeable` 去掉路径末尾分隔符 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4218](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4218) | 复用中断的 checkpoint id |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4282](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4282) | 空 scores 时 `accuracy()` 返回 0 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#4090](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4090) | 澄清 model-graded history prompt：`include_history=True` 和最终答案字段的位置与实际 scorer 行为保持一致 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#3982](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3982) | 在 agent bridge 转换里保留 wrapped 的 OpenAI reasoning payload，加密的 provider 原生 reasoning 项在 transcript 转换时不丢。 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#3896](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3896) | 修复 filestore recovery append 模式：保留已恢复 message/tool-call 池，同时避免重复哈希旧片段 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#3902](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3902) | 修复 OpenAI-compatible 响应里的 OpenRouter `reasoning_details`：解析为可读 reasoning 文本，而不是暴露 Python repr |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.5k★) | [#3895](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3895) | 修复 `TERM=dumb` 下终端宽度：尊重 `COLUMNS`，日志输出不再固定按 Rich 默认 80 列硬换行 |
| [LMCache](https://github.com/LMCache/LMCache) (11.1k★) | [#3245](https://github.com/LMCache/LMCache/pull/3245) | MP store/retrieve 期间留住 producer 侧的 CUDA IPC event，别让 daemon 拿着已回收的 handle 去恢复。 |
| [LMCache](https://github.com/LMCache/LMCache) (11.1k★) | [#3282](https://github.com/LMCache/LMCache/pull/3282) | MP KV transfer 处理 HND 这种 GPU KV layout，之前这种排布会被算错。 |
| [FastMCP](https://github.com/PrefectHQ/fastmcp) (27.1k★) | [#4297](https://github.com/PrefectHQ/fastmcp/pull/4297) | 构建工具 schema 时保留必需的 discriminator tag，union 参数才还有效。 |
| [FlashInfer](https://github.com/flashinfer-ai/flashinfer) (6.1k★) | [#2772](https://github.com/flashinfer-ai/flashinfer/pull/2772) | 修复编译错误：CUTLASS 头文件缺少 `<optional>` include 导致 `std::optional` 未定义 |
| [FlashInfer](https://github.com/flashinfer-ai/flashinfer) (6.1k★) | [#2756](https://github.com/flashinfer-ai/flashinfer/pull/2756) | 修复 autotuner 在输入 tensor 为 `None` 时崩溃（fixes #2749） |
| [MCP Toolbox](https://github.com/googleapis/mcp-toolbox) (16.1k★) | [#3738](https://github.com/googleapis/mcp-toolbox/pull/3738) | execute_sql 保留 BigQuery 原生错误分类，模拟服务账号的 403 按客户端错误上报告别笼统 500 |
| [MCP Toolbox](https://github.com/googleapis/mcp-toolbox) (16.1k★) | [#3516](https://github.com/googleapis/mcp-toolbox/pull/3516) | 参数 type 字段不是字符串时返回错误，而不是 panic |
| [MCP Toolbox](https://github.com/googleapis/mcp-toolbox) (16.1k★) | [#3512](https://github.com/googleapis/mcp-toolbox/pull/3512) | array/map 参数类型报错时带上导致出错的具体值 |
| [MCP Toolbox](https://github.com/googleapis/mcp-toolbox) (16.1k★) | [#3416](https://github.com/googleapis/mcp-toolbox/pull/3416) | 补充 execute_sql 最小权限配置的文档 |
| [MCP Toolbox](https://github.com/googleapis/mcp-toolbox) (16.1k★) | [#3531](https://github.com/googleapis/mcp-toolbox/pull/3531) | 校验 Looker explore_references 的结构，非法输入不再 panic |
| [Pydantic AI](https://github.com/pydantic/pydantic-ai) (19.1k★) | [#5695](https://github.com/pydantic/pydantic-ai/pull/5695) | 在 completions 里转发 penalties 参数 |
| [Pydantic AI](https://github.com/pydantic/pydantic-ai) (19.1k★) | [#5694](https://github.com/pydantic/pydantic-ai/pull/5694) | 修复 `MCPToolset(http_client=...)` 与 FastMCP 的兼容问题，避免把 `follow_redirects` 泄漏给调用方提供的 HTTP client factory |
| [Pydantic AI](https://github.com/pydantic/pydantic-ai) (19.1k★) | [#5474](https://github.com/pydantic/pydantic-ai/pull/5474) | 接受 Vercel AI dynamic-tool 消息里的 `providerExecuted` 和 `title`，严格校验下也留住 provider 元数据。 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13637](https://github.com/Arize-ai/phoenix/pull/13637) | in-memory SQLite schema 初始化完再对外服务 Phoenix，启动竞态撞不上缺表。 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13641](https://github.com/Arize-ai/phoenix/pull/13641) | provider 变化时让 prompt tool diff 过期，PXI 编辑不再把旧的工具差异状态带到别的 provider。 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13245](https://github.com/Arize-ai/phoenix/pull/13245) | 修复 generative model fetch 游标回退：低 id 更新不会让后续轮询跳过更新的模型变更 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13242](https://github.com/Arize-ai/phoenix/pull/13242) | 为 raw computer tool definitions 传递 Anthropic computer-use beta headers，覆盖 playground streaming 和非 streaming 调用 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13210](https://github.com/Arize-ai/phoenix/pull/13210) | 修复非法 GraphQL node id 的错误处理：返回 NotFound 风格错误，而不是把 decoder failure 泄漏给客户端 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13261](https://github.com/Arize-ai/phoenix/pull/13261) | 修复 span annotation note 新建后的刷新问题：创建成功后立即重新拉取列表，前端不再需要手动刷新才能看到新 note |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13533](https://github.com/Arize-ai/phoenix/pull/13533) | span 标注工具的空输入给出明确处理，不再模糊失败 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13636](https://github.com/Arize-ai/phoenix/pull/13636) | 更新 PXI system prompt 指南，指向当前 server-side Jinja 模板和 capability wiring，不再引用过期的 browser-side 路径 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13653](https://github.com/Arize-ai/phoenix/pull/13653) | PXI agent 面板一打开就聚焦输入框，键盘优先的流程少点一下。 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13614](https://github.com/Arize-ai/phoenix/pull/13614) | 修复 Prompts 表格停留页面时不会自动刷新的问题：新建或更新的 prompt 不再需要手动刷新才能出现 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.9k★) | [#13139](https://github.com/Arize-ai/phoenix/pull/13139) | 修复 Playground 校验错误被吞掉的问题：失败时返回明确错误，而不是空 subscription payload |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2823](https://github.com/strands-agents/harness-sdk/pull/2823) | 空 model stream 时避免 `UnboundLocalError` |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2400](https://github.com/strands-agents/harness-sdk/pull/2400) | 支持非流式 OpenAI chat completions |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2340](https://github.com/strands-agents/harness-sdk/pull/2340) | 并发的 tool result 按请求顺序回填，并行执行不会打乱模型看到的输出顺序。 |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2354](https://github.com/strands-agents/harness-sdk/pull/2354) | 读 OpenAI 兼容 vLLM 流里的 `delta.reasoning`，reasoning 输出过了 provider 转换也不丢。 |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2353](https://github.com/strands-agents/harness-sdk/pull/2353) | 处理 Gemini safety-blocked metadata：缺失 token 计数时安全归零，并把 safety stop 映射为 guardrail intervention |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2306](https://github.com/strands-agents/harness-sdk/pull/2306) | 规范化 3gp 视频格式 |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2304](https://github.com/strands-agents/harness-sdk/pull/2304) | 显式映射 webp 图片 |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2656](https://github.com/strands-agents/harness-sdk/pull/2656) | 处理空的 Bedrock content block |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.8k★) | [#2396](https://github.com/strands-agents/harness-sdk/pull/2396) | 传递 structured output 的请求参数 |
| [LightRAG](https://github.com/HKUDS/LightRAG) (38.6k★) | [#3206](https://github.com/HKUDS/LightRAG/pull/3206) | PostgreSQL 表存在性检查尊重 `search_path`，非 public schema 在迁移、建表前就能识别对。 |
| [LightRAG](https://github.com/HKUDS/LightRAG) (38.6k★) | [#3031](https://github.com/HKUDS/LightRAG/pull/3031) | 从 Docling 异步结果 envelope 里抽出 Markdown 正文，RAG chunk 拿到干净文本，不混 JSON/base64 噪声。 |
| [LightRAG](https://github.com/HKUDS/LightRAG) (38.6k★) | [#2796](https://github.com/HKUDS/LightRAG/pull/2796) | 修复 `None` file_path 传播为 `unknown_source`：补 #2793 遗漏的处理层 |
| [LightRAG](https://github.com/HKUDS/LightRAG) (38.6k★) | [#3123](https://github.com/HKUDS/LightRAG/pull/3123) | 把 API 文档配色和暗色主题同步，endpoint 示例在 dark mode 下也读得清。 |
| [Pipecat](https://github.com/pipecat-ai/pipecat) (14.0k★) | [#4766](https://github.com/pipecat-ai/pipecat/pull/4766) | DTMF 缓存键补上采样率，同一按键不同采样率的提示音不再互相串音 |
| [Pipecat](https://github.com/pipecat-ai/pipecat) (14.0k★) | [#4553](https://github.com/pipecat-ai/pipecat/pull/4553) | 修复 protobuf transport 丢失 interruption frame：实时语音 agent 的打断事件跨传输后仍能保留 |
| [Graphiti](https://github.com/getzep/graphiti) (29.7k★) | [#1531](https://github.com/getzep/graphiti/pull/1531) | 递归清掉 FalkorDB 查询参数里的 NUL 字节，单个异常文档字符串打断不了批量图写入。 |
| [Kimi Code](https://github.com/MoonshotAI/kimi-code) (6.2k★) | [#2255](https://github.com/MoonshotAI/kimi-code/pull/2255) | 通过 status_line 配置自定义 TUI 底部状态栏（仿 codex / claude code 的 footer 形态） |
| [OpenHarness](https://github.com/HKUDS/OpenHarness) (15.3k★) | [#185](https://github.com/HKUDS/OpenHarness/pull/185) | TUI tab 补全三合一修复：光标跳回、去除尾部空格、接受 `/quit` 别名 |
| [LM Evaluation Harness](https://github.com/EleutherAI/lm-evaluation-harness) (13.6k★) | [#3822](https://github.com/EleutherAI/lm-evaluation-harness/pull/3822) | 保证传给 Anthropic 的 stop sequence 非空，避免请求被拒 |
| [MCP Registry](https://github.com/modelcontextprotocol/registry) (7.1k★) | [#1310](https://github.com/modelcontextprotocol/registry/pull/1310) | 拒绝损坏的 publisher 元数据，而不是接收畸形条目 |
| [ClawTeam](https://github.com/HKUDS/ClawTeam) (5.5k★) | [#32](https://github.com/HKUDS/ClawTeam/pull/32) | Gemini CLI 支持：spawn、权限、prompt 注入双 backend 适配 |
| [ClawTeam](https://github.com/HKUDS/ClawTeam) (5.5k★) | [#36](https://github.com/HKUDS/ClawTeam/pull/36) | Kimi CLI 支持：spawn backend、权限处理、3 个新测试 |
| [ClawTeam](https://github.com/HKUDS/ClawTeam) (5.5k★) | [#40](https://github.com/HKUDS/ClawTeam/pull/40) | 可插拔 TaskStore：将任务持久化抽取为可替换的后端抽象层 |
| [ClawTeam](https://github.com/HKUDS/ClawTeam) (5.5k★) | [#1](https://github.com/HKUDS/ClawTeam/pull/1) | 首个 PR：122 个测试、CI、团队模板、config 修复、任务耗时追踪 |
| [MCP Go SDK](https://github.com/modelcontextprotocol/go-sdk) (4.9k★) | [#962](https://github.com/modelcontextprotocol/go-sdk/pull/962) | 拒绝重复的 `initialize` 请求，MCP session 初始化后的协议状态保持一致。 |
| [MCP Go SDK](https://github.com/modelcontextprotocol/go-sdk) (4.9k★) | [#981](https://github.com/modelcontextprotocol/go-sdk/pull/981) | 补齐 `Implementation.description` 元数据，同时让空描述继续不进入序列化后的 MCP payload |
| [Microsoft Recommenders](https://github.com/recommenders-team/recommenders) (21.9k★) | [#2345](https://github.com/recommenders-team/recommenders/pull/2345) | 先用 PyTorch 查 GPU 显存，numba 兜底，CUDA context 不可用时 GPU discovery 不至于直接失败。 |
| [Microsoft Recommenders](https://github.com/recommenders-team/recommenders) (21.9k★) | [#2351](https://github.com/recommenders-team/recommenders/pull/2351) | TensorFlow GPU 不可用时 fail fast |
| [Microsoft Recommenders](https://github.com/recommenders-team/recommenders) (21.9k★) | [#2349](https://github.com/recommenders-team/recommenders/pull/2349) | 优先用 torch 查询 GPU 显存 |
| [Microsoft Recommenders](https://github.com/recommenders-team/recommenders) (21.9k★) | [#2322](https://github.com/recommenders-team/recommenders/pull/2322) | 让 benchmark 的推荐数量参数生效，评测脚本按要求生成 top-k。 |
| [Microsoft Recommenders](https://github.com/recommenders-team/recommenders) (21.9k★) | [#2350](https://github.com/recommenders-team/recommenders/pull/2350) | 统一标注 MAP@k notebook 的输出 |
| [DB-GPT](https://github.com/eosphoros-ai/DB-GPT) (19.7k★) | [#3092](https://github.com/eosphoros-ai/DB-GPT/pull/3092) | sandbox 用本地 runtime 执行前要求显式 opt-in |
| [Google Gen AI SDK](https://github.com/googleapis/python-genai) (3.9k★) | [#2564](https://github.com/googleapis/python-genai/pull/2564) | 让 Live Music API key 不再进入 websocket URL query，改由请求 header 承载，避免密钥出现在日志和代理路径里 |
| [yfinance](https://github.com/ranaroussi/yfinance) (24.9k★) | [#2867](https://github.com/ranaroussi/yfinance/pull/2867) | 补上漏掉的逗号，避免 equity screener 的两个 EPS 字段被并成一个 |
| [EvalScope](https://github.com/modelscope/evalscope) (3.2k★) | [#1381](https://github.com/modelscope/evalscope/pull/1381) | 从 OpenAI 风格的 text content block 里读 SciCode 的 assistant 答案，scorer prompt 拿到真答案而不是空字段。 |
| [OpenHands SDK](https://github.com/OpenHands/software-agent-sdk) (971★) | [#3248](https://github.com/OpenHands/software-agent-sdk/pull/3248) | 用 RLock 串行化 LiteLLM `modify_params` 的保存、设置和恢复，避免并发 completion 泄漏全局参数状态 |
| [OpenHands SDK](https://github.com/OpenHands/software-agent-sdk) (971★) | [#3247](https://github.com/OpenHands/software-agent-sdk/pull/3247) | 用 `git rev-parse --git-dir` 校验 git workspace，坏掉的嵌套 repo 打不崩 `/api/git/changes`。 |
| [OpenHands SDK](https://github.com/OpenHands/software-agent-sdk) (971★) | [#3225](https://github.com/OpenHands/software-agent-sdk/pull/3225) | remote completion 日志按 UTF-8 写，中文和非 ASCII 输出在本地回放、排查时不乱码。 |

### 领英LinkedIn: https://www.linkedin.com/in/yufenghe
