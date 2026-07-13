## Hey, I'm Yufeng He 👋

AI Agents & LLM Systems Engineer | Formerly @ [Moonshot AI](https://www.moonshot.ai/) (Kimi) | MS CS @ HKU | Champion, Shanghai Global AI Contest | 3x ACM-ICPC Silver Medalist | Former Intern @ Baidu, Maimai, Kuaishou

- 200+ merged upstream PRs, with fixes in vLLM (9 merged), Mooncake (24 merged), Qwen Code (51 merged), Microsoft Agent Framework (20 merged), AstrBot (30 merged), Google ADK (10 merged), Inspect AI (18 merged), Hugging Face Transformers (1 merged), and PyTorch (3 merged).
- Selected public projects led by CoreCoder, FindJobs-Agent, RepoWiki, and ContractGuard.

### Projects

| Area | Project | Stars | Notes |
|------|---------|:-----:|-------|
| Coding agents / evals | [CoreCoder](https://github.com/he-yufeng/CoreCoder) | 1.5k+ | 512K lines of Claude Code → 1,400 lines of Python. Every key architectural pattern, runnable. Any LLM. 7 architecture deep-dive articles. |
| Applied agents | [FindJobs-Agent](https://github.com/he-yufeng/FindJobs-Agent) | 200+ | LLM-powered job toolkit: skill gap analysis, mock interviews, resume optimization, and job structuring. |
| Codebase maps | [RepoWiki](https://github.com/he-yufeng/RepoWiki) | 200+ | Open-source DeepWiki alternative: CLI/browser wiki generation, PageRank file ranking, Mermaid diagrams, and reading guides. |
| Applied agents | [ContractGuard](https://github.com/he-yufeng/ContractGuard) | 100+ | AI agent that reviews contracts for red flags before you sign: unfair terms, missing protections, and plain-English explanations. |
| Codebase maps | [GitSense](https://github.com/he-yufeng/GitSense) | 100+ | AI-powered contribution finder and repo radar: find matching issues, then check PR merge signals before spending a weekend. |
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

#### AI infrastructure / model systems

| Project | PR | What I Fixed |
|---------|:--:|-------------|
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#37884](https://github.com/vllm-project/vllm/pull/37884) | RoBERTa position_ids in-place accumulation on CUDA graph padding: BGE-M3 crash after ~4000 requests |
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#40789](https://github.com/vllm-project/vllm/pull/40789) | Support tuple model outputs in the V1 ubatch wrapper so DBO and speculative decoding stop crashing on tuple-returning models |
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#44821](https://github.com/vllm-project/vllm/pull/44821) | Prefix DeepSeek V4 MTP projection layers so compressed-tensors can match artifact-side target and ignore rules during draft model loading |
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#43243](https://github.com/vllm-project/vllm/pull/43243) | Parse Qwen3 XML tool-call parameters as JSON first so `null` / `false` survive streaming tool parsing instead of being rejected by Python literal parsing |
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#37727](https://github.com/vllm-project/vllm/pull/37727) | Fix Responses API `instructions` leaking across turns via `previous_response_id` chain |
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#42679](https://github.com/vllm-project/vllm/pull/42679) | Guard flash-attn rotary imports so FA4 environments fall back cleanly when `flash_attn.ops.triton.rotary` is absent |
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#37699](https://github.com/vllm-project/vllm/pull/37699) | Fix weight offloading ignoring `VLLM_WEIGHT_OFFLOADING_DISABLE_PIN_MEMORY` in prefetch offloader |
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#37301](https://github.com/vllm-project/vllm/pull/37301) | Base64 JPEG video frames returning empty metadata: populate frame count, fps, duration |
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#38732](https://github.com/vllm-project/vllm/pull/38732) | Fix bench_serve UTF-8 decode crash on split multi-byte chars in streaming chunks |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#1629](https://github.com/kvcache-ai/Mooncake/pull/1629) | GB200 MNNVL EP hang: `cudaMalloc` → `cuMemCreate(FABRIC)` + `cuMemMap` for cross-node NVLink |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#2570](https://github.com/kvcache-ai/Mooncake/pull/2570) | Integer overflow in `BatchOffload` for >4 GiB objects: sum slice sizes in `uint64_t` and reject objects exceeding the `uint32_t` record `value_len`, instead of silently truncating |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#2610](https://github.com/kvcache-ai/Mooncake/pull/2610) | Restore the `task.request` association in `RdmaTransport::submitTransfer`: a refactor dropped the per-task `request` pointer, leaving every downstream task with null and breaking status/retry/accounting reads |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#1728](https://github.com/kvcache-ai/Mooncake/pull/1728) | Hard pin for eviction-protected objects: model weights never get evicted, const field + BatchEvict skip + backward-compat serialization |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#1719](https://github.com/kvcache-ai/Mooncake/pull/1719) | Add `ObjectDataType` metadata classification for KV cache, weights, tensors, and snapshots, with backward-compatible serialization and Python bindings |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#1831](https://github.com/kvcache-ai/Mooncake/pull/1831) | TENT NVLink IPC fix: use base pointer for sub-allocated GPU tensors, porting #1622 fix to TENT path |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#1644](https://github.com/kvcache-ai/Mooncake/pull/1644) | MNNVL warmup hang: skip redundant handshake for fabric-connected nodes |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#1825](https://github.com/kvcache-ai/Mooncake/pull/1825) | Fix `P2PClientService::Put` silently swallowing write errors: propagate actual error codes for non-idempotent failures |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#2402](https://github.com/kvcache-ai/Mooncake/pull/2402) | Reject failed Python buddy-allocator backing buffers instead of inserting null raw buffers into managed slabs |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#2403](https://github.com/kvcache-ai/Mooncake/pull/2403) | Clean up failed io_uring sub-batch initialization so partially prepared transfer batches do not leak failed state into later setup |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#2311](https://github.com/kvcache-ai/Mooncake/pull/2311) | Make duplicate `rpc_meta` re-publish idempotent when the HTTP metadata body is unchanged, while still rejecting changed values |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#1626](https://github.com/kvcache-ai/Mooncake/pull/1626) | Silenced error log spam for non-memory replicas in metadata store |
| [Transformers](https://github.com/huggingface/transformers) (162.5k★) | [#44710](https://github.com/huggingface/transformers/pull/44710) | Fix `AutoProcessor.from_pretrained` silently dropping hub kwargs (`revision`, `token`, etc.) |
| [PyTorch](https://github.com/pytorch/pytorch) (101.8k★) | [#176100](https://github.com/pytorch/pytorch/pull/176100) | Fix user-defined Triton kernel name mangling in the Inductor codegen so distinct kernels stop colliding in generated code (shows as Closed; landed via pytorchmergebot) |
| [PyTorch](https://github.com/pytorch/pytorch) (101.8k★) | [#187643](https://github.com/pytorch/pytorch/pull/187643) | Fix a `ValueError` in the `stale_issues` workflow's `parse_older_than` on non-leap years, where a naive Feb 29 offset crashed the run (shows as Closed; landed via pytorchmergebot) |
| [PyTorch](https://github.com/pytorch/pytorch) (101.8k★) | [#187262](https://github.com/pytorch/pytorch/pull/187262) | Remove the obsolete `setuptools` upper bound so builds resolve a current toolchain instead of pinning a stale one (shows as Closed; landed via pytorchmergebot) |
| [LiteLLM](https://github.com/BerriAI/litellm) (51.4k★) | [#26401](https://github.com/BerriAI/litellm/pull/26401) | Fix `LITELLM_LOG=INFO` missing `verbose_logger`: proxy INFO logs now include all verbose logger sources |
| [SGLang](https://github.com/sgl-project/sglang) (30.2k★) | [#20739](https://github.com/sgl-project/sglang/pull/20739) | Fix hybrid_linear_attn_backend crash when used with ngram speculative decoding |
| [verl](https://github.com/verl-project/verl) (22.4k★) | [#6620](https://github.com/verl-project/verl/pull/6620) | Derive colocated vLLM weight-sync ZMQ socket ranks from data-parallel and tensor-parallel ranks so DP workers do not collide on the same receiver |
| [Triton](https://github.com/triton-lang/triton) (19.7k★) | [#9613](https://github.com/triton-lang/triton/pull/9613) | Fix AxisInfo correctness: signed constants, unknown shift divisibility, and shift UB guards |
| [TRL](https://github.com/huggingface/trl) (18.8k★) | [#6054](https://github.com/huggingface/trl/pull/6054) | Reject already-transformed datasets during SFT preparation so misconfigured runs fail fast instead of silently producing wrong training batches |
| [LMCache](https://github.com/LMCache/LMCache) (9.8k★) | [#3245](https://github.com/LMCache/LMCache/pull/3245) | Retain producer-side CUDA IPC events during MP store/retrieve requests so daemon IPC handles do not point at collected events |
| [LMCache](https://github.com/LMCache/LMCache) (9.8k★) | [#3282](https://github.com/LMCache/LMCache/pull/3282) | Support HND GPU KV formats in MP KV transfer so alternate KV tensor layouts are handled correctly |
| [FlashInfer](https://github.com/flashinfer-ai/flashinfer) (5.9k★) | [#2756](https://github.com/flashinfer-ai/flashinfer/pull/2756) | Fix autotuner crash when input tensor is `None`: proper None-checking for optional inputs (fixes #2749) |
| [FlashInfer](https://github.com/flashinfer-ai/flashinfer) (5.9k★) | [#2772](https://github.com/flashinfer-ai/flashinfer/pull/2772) | Fix compilation error: add missing `<optional>` header for `std::optional` usage in CUTLASS headers |
| [Google Gen AI SDK](https://github.com/googleapis/python-genai) (3.8k★) | [#2564](https://github.com/googleapis/python-genai/pull/2564) | Keep Live Music API keys out of websocket URLs by relying on request headers instead of duplicating secrets in query strings |

#### Agent frameworks / protocols / evals

| Project | PR | What I Fixed |
|---------|:--:|-------------|
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5036](https://github.com/QwenLM/qwen-code/pull/5036) | Hard-stop repeated identical tool calls so an agent cannot keep executing the same stalled action after loop detection fires |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5020](https://github.com/QwenLM/qwen-code/pull/5020) | Drop tool calls after cancellation so aborted turns do not leak stale tool requests into the next provider payload |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4622](https://github.com/QwenLM/qwen-code/pull/4622) | Keep assistant tool calls adjacent to their tool results so OpenAI-compatible providers stop rejecting repaired message histories |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5071](https://github.com/QwenLM/qwen-code/pull/5071) | Submit fast tool results after stream end so completed calls do not get stranded by a race at the end of model streaming |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4970](https://github.com/QwenLM/qwen-code/pull/4970) | Stabilize truncated tool retry keys so repaired tool calls keep deterministic retry identity instead of drifting across retries |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5058](https://github.com/QwenLM/qwen-code/pull/5058) | Avoid stale tool-schema recall so memory warnings do not reintroduce outdated tool names into later planning turns |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5062](https://github.com/QwenLM/qwen-code/pull/5062) | Preserve token-escalation context across agent rounds so delegated runs do not repeatedly restart from an under-provisioned model |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4828](https://github.com/QwenLM/qwen-code/pull/4828) | Preserve a user-provided shared `baseUrl` after auth refresh so same-model refreshes do not fall back to a provider default endpoint |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4829](https://github.com/QwenLM/qwen-code/pull/4829) | Time out Qwen OAuth refresh requests so auth recovery does not hang the CLI indefinitely on a stalled refresh endpoint |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4607](https://github.com/QwenLM/qwen-code/pull/4607) | Fix IDE proxy requests by keeping `fetch` and `EnvHttpProxyAgent` on the same bundled `undici` module path |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4716](https://github.com/QwenLM/qwen-code/pull/4716) | Route `/bug`, `/docs`, and `/insight` browser launches through the secure opener so headless environments do not crash on direct `open` calls |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4596](https://github.com/QwenLM/qwen-code/pull/4596) | Recurse into tracked Git submodules during repository crawling so coding-agent context includes files inside submodules |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5115](https://github.com/QwenLM/qwen-code/pull/5115) | Hide teammate-only agent names when teams are disabled and fall back to one-shot subagents if an old prompt still sends one |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5070](https://github.com/QwenLM/qwen-code/pull/5070) | Ignore expired live agents in focus navigation so stale background-agent rows cannot steal keyboard focus |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5061](https://github.com/QwenLM/qwen-code/pull/5061) | Preserve background-agent launch flags so delegated CLI runs keep the intended execution mode |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4715](https://github.com/QwenLM/qwen-code/pull/4715) | Honor the configured runtime output directory for managed auto-memory while preserving the explicit memory-directory override |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4717](https://github.com/QwenLM/qwen-code/pull/4717) | Replace exit-time deep history clones with shallow read paths across copy, arena, and ACP snapshot flows while keeping restore-time cloning defensive |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5043](https://github.com/QwenLM/qwen-code/pull/5043) | Let grep results satisfy prior-read checks so file edits can proceed after verified search context instead of forcing redundant reads |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4673](https://github.com/QwenLM/qwen-code/pull/4673) | Restore top-level `--list-extensions` / `-l` so it prints installed extensions and exits before sandbox, auth, or TUI startup |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4632](https://github.com/QwenLM/qwen-code/pull/4632) | Harden context-error text collection so nested/non-string error payloads surface useful messages instead of disappearing |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5077](https://github.com/QwenLM/qwen-code/pull/5077) | Show the full plan when permission gates fail so users can inspect blocked agent intent instead of losing the generated plan |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5073](https://github.com/QwenLM/qwen-code/pull/5073) | Warn when context instruction files exceed the configured budget so oversized repository guidance is visible before it silently crowds out task context |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4963](https://github.com/QwenLM/qwen-code/pull/4963) | Enable fork subagents by default so delegated work can run in isolated branches without manual opt-in |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4600](https://github.com/QwenLM/qwen-code/pull/4600) | Distinguish AUTO from AUTO_EDIT approval-mode indicators in the TUI, including shared styling, i18n keys, and visual evidence |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4738](https://github.com/QwenLM/qwen-code/pull/4738) | Skip hidden thought parts when copying visible CLI output so clipboard exports match what users actually see |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4639](https://github.com/QwenLM/qwen-code/pull/4639) | Drop the discontinued Qwen OAuth path from ACP login so users are not routed into a dead authentication method |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4636](https://github.com/QwenLM/qwen-code/pull/4636) | Apply the requested output language to side queries so auxiliary answers follow the same language contract as the main response |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4635](https://github.com/QwenLM/qwen-code/pull/4635) | Hide completed sticky todos from the active CLI todo view so persistent task hints stay focused on remaining work |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5072](https://github.com/QwenLM/qwen-code/pull/5072) | Stabilize the simple MCP integration check so transient server readiness timing no longer makes the cross-process contract test flaky |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5462](https://github.com/microsoft/agent-framework/pull/5462) | Fix `background=True` + tools infinite-retrieve loop: clear completed continuation state so tool results get posted |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5773](https://github.com/microsoft/agent-framework/pull/5773) | Run synchronous Python tools off the event loop so blocking tool calls no longer freeze concurrent agent work |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#6210](https://github.com/microsoft/agent-framework/pull/6210) | Drop hosted MCP tool-call history when reasoning payloads are stripped so stateless OpenAI replay does not send orphan MCP calls |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#6132](https://github.com/microsoft/agent-framework/pull/6132) | Filter filesystem checkpoint indexes by session id so reopened stores do not return checkpoints from other workflow sessions |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5904](https://github.com/microsoft/agent-framework/pull/5904) | Keep ChatClientAgent's local history provider active for AG-UI thread ids so session history is not mistaken for service-managed model history |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#6208](https://github.com/microsoft/agent-framework/pull/6208) | Preserve full PowerFx record values in declarative `Foreach` loops so multi-field table rows do not collapse during iteration |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5861](https://github.com/microsoft/agent-framework/pull/5861) | Preserve structured Foundry handoff arguments so delegated agent calls survive response conversion |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5808](https://github.com/microsoft/agent-framework/pull/5808) | Fix handoff message role mutation so retries reuse sanitized messages without leaking role changes |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5784](https://github.com/microsoft/agent-framework/pull/5784) | Skip orphan Anthropic thinking signatures when converting history so replayed messages do not carry invalid standalone signatures |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5778](https://github.com/microsoft/agent-framework/pull/5778) | Declare Magentic protocol messages so orchestrator chat/reset signals deserialize instead of failing on unknown types |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5800](https://github.com/microsoft/agent-framework/pull/5800) | Avoid AG-UI tool result message id collisions when providers omit update ids |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5801](https://github.com/microsoft/agent-framework/pull/5801) | Coalesce streamed code interpreter history chunks by call id so final stored history keeps complete code/results without duplicate deltas |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5974](https://github.com/microsoft/agent-framework/pull/5974) | Include Foundry agent tool definitions in eval mappings so evaluator runs can call code-defined tools |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#6037](https://github.com/microsoft/agent-framework/pull/6037) | Keep Foundry citation `get_url` metadata through response conversion so source links survive in chat responses |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#6040](https://github.com/microsoft/agent-framework/pull/6040) | Forward Foundry agent `default_headers` into OpenAI client creation so custom auth and routing headers survive agent setup |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5815](https://github.com/microsoft/agent-framework/pull/5815) | Forward MCP tool-call metadata from `tools/list` into `call_tool` instrumentation so traces keep tool annotations |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5799](https://github.com/microsoft/agent-framework/pull/5799) | Add handoff workflow naming metadata so names and descriptions flow through builder and hosting registration |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5976](https://github.com/microsoft/agent-framework/pull/5976) | Fix sequential workflow sample output so all participant responses are shown from non-streaming results |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#6474](https://github.com/AstrBotDevs/AstrBot/pull/6474) | SQLite `database is locked` under concurrent writes: added busy timeout |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#6596](https://github.com/AstrBotDevs/AstrBot/pull/6596) | Multimodal token counting: images, audio, chain-of-thought were invisible to context compression |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#7003](https://github.com/AstrBotDevs/AstrBot/pull/7003) | SSE heartbeat for WebChat: long context compression killed the connection |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#6581](https://github.com/AstrBotDevs/AstrBot/pull/6581) | Context truncation dropping the only user message: causes 400 from Zhipu/Gemini |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#7216](https://github.com/AstrBotDevs/AstrBot/pull/7216) | Fix Gemini tool call 400: wrap plain-text tool results as Protobuf Struct |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#6313](https://github.com/AstrBotDevs/AstrBot/pull/6313) | Null choices guard: OpenAI API returning `None` instead of empty list |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#6551](https://github.com/AstrBotDevs/AstrBot/pull/6551) | Fix empty content causing Grok 400: set content to None when empty |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#7407](https://github.com/AstrBotDevs/AstrBot/pull/7407) | Fix Gemini native search 400 when no function tools: skip FunctionCallingConfig |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#7196](https://github.com/AstrBotDevs/AstrBot/pull/7196) | Fix Gemini thinking parts leaking into user-facing response |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#7758](https://github.com/AstrBotDevs/AstrBot/pull/7758) | Apply empty-assistant message filter to streaming OpenAI path: strict providers no longer 400 on reasoning-only turns |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8089](https://github.com/AstrBotDevs/AstrBot/pull/8089) | Route image requests to a vision-capable fallback provider when the primary provider cannot accept image input |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8119](https://github.com/AstrBotDevs/AstrBot/pull/8119) | Pass image inputs through active replies so image-triggered mentions reach the LLM as image URLs |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8073](https://github.com/AstrBotDevs/AstrBot/pull/8073) | Fix image-only KB retrieval: skip blank prompts so embedding APIs are not called with empty text |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#6710](https://github.com/AstrBotDevs/AstrBot/pull/6710) | Skills-like re-query dropping image captions: `extra_user_content_parts` not forwarded |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8195](https://github.com/AstrBotDevs/AstrBot/pull/8195) | Skip empty LLM summaries so context compression keeps the original history instead of inserting blank placeholders |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#7537](https://github.com/AstrBotDevs/AstrBot/pull/7537) | Prevent Telegram media group exceptions from being silently swallowed by APScheduler |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#7398](https://github.com/AstrBotDevs/AstrBot/pull/7398) | Fix Telegram sendMessageDraft spamming 400 errors on empty text in streaming mode |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8175](https://github.com/AstrBotDevs/AstrBot/pull/8175) | Surface WeChat OA media send failures instead of reporting success after prepare/send timeouts |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#6656](https://github.com/AstrBotDevs/AstrBot/pull/6656) | `/stop` follow-up race: agent_stop flag not checked during follow-up capture |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8061](https://github.com/AstrBotDevs/AstrBot/pull/8061) | Keep Discord startup alive when command sync hits the daily create quota; only quota errors become warnings |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#7217](https://github.com/AstrBotDevs/AstrBot/pull/7217) | Fix qwen3-rerank response parsing: handle both old and new Dashscope API formats |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8768](https://github.com/AstrBotDevs/AstrBot/pull/8768) | Sanitize Lark platform id suffixes so invisible whitespace in configured ids does not break platform matching |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8736](https://github.com/AstrBotDevs/AstrBot/pull/8736) | Preserve embedding API version suffixes so versioned provider endpoints do not get normalized into the wrong path |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8255](https://github.com/AstrBotDevs/AstrBot/pull/8255) | Support RST and AsciiDoc knowledge uploads by keeping backend parser checks and dashboard file validation in sync |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8718](https://github.com/AstrBotDevs/AstrBot/pull/8718) | Avoid duplicate quoted image captions when multimodal replies include both quoted text and image metadata |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8172](https://github.com/AstrBotDevs/AstrBot/pull/8172) | Prefer bundled dashboard assets over stale data dist so releases do not serve an outdated WebUI |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#6527](https://github.com/AstrBotDevs/AstrBot/pull/6527) | Fix LLM tool selection: rewrote ambiguous Upload/Download descriptions |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8750](https://github.com/AstrBotDevs/AstrBot/pull/8750) | Resolve changelog anchor links so dashboard release notes navigate to the intended section instead of broken anchors |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8388](https://github.com/AstrBotDevs/AstrBot/pull/8388) | Add missing dashboard i18n for plugin sub-command counts so extension details stop showing raw translation keys |
| [Google ADK](https://github.com/google/adk-python) (20.3k★) | [#5698](https://github.com/google/adk-python/pull/5698) | Include intermediate responses in `final_response_match_v2` judging when the criterion opts in |
| [Google ADK](https://github.com/google/adk-python) (20.3k★) | [#5918](https://github.com/google/adk-python/pull/5918) | Allow the builder assistant's internal app name through CLI runner validation so `adk web` can open the special agent |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#3896](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3896) | Fix filestore recovery append mode: preserve carried message/tool-call pools without rehashing old segments |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#3982](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3982) | Preserve wrapped OpenAI reasoning payloads in the agent bridge so encrypted provider-native reasoning items survive transcript conversion |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#3975](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3975) | Preserve call-site generation defaults when role model overrides are resolved, so eval roles can switch models without dropping config like max tokens or reasoning effort |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#4069](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4069) | Flush streamed score samples periodically so long-running eval streams persist score rows before final completion |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#3924](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3924) | Reject unknown `GenerateConfig` fields early so misspelled generation options do not get silently ignored |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#3941](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3941) | Route Bedrock Nova `top_k` through the inference config instead of dropping the sampling control |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#3902](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3902) | Parse OpenRouter `reasoning_details` in OpenAI-compatible responses instead of surfacing Python repr blocks |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#3895](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3895) | Honor `COLUMNS` for `TERM=dumb`: log output no longer hard-wraps at Rich's default 80 columns |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#4090](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4090) | Clarify model-graded history prompts so `include_history=True` and final-answer placement match the actual scorer behavior |
| [OpenClaw](https://github.com/openclaw/openclaw) (380.3k★) | [#41259](https://github.com/openclaw/openclaw/pull/41259) | Propagate memory directory creation failures instead of continuing after a failed `ensureDir` |
| [OpenClaw](https://github.com/openclaw/openclaw) (380.3k★) | [#41271](https://github.com/openclaw/openclaw/pull/41271) | Log auth profile resolution failures instead of swallowing silently |
| [OpenHands](https://github.com/OpenHands/OpenHands) (78.3k★) | [#14776](https://github.com/OpenHands/OpenHands/pull/14776) | Preserve custom LLM base URLs when editing basic model settings so saved profiles do not silently fall back to provider defaults |
| [Cline](https://github.com/cline/cline) (63.9k★) | [#11166](https://github.com/cline/cline/pull/11166) | Keep file search alive when the open-tabs host RPC is unavailable, falling back to system ripgrep instead of killing search |
| [Mem0](https://github.com/mem0ai/mem0) (59.4k★) | [#5416](https://github.com/mem0ai/mem0/pull/5416) | Use valid S3 Vectors entity index names so agent memory writes no longer hit AWS index-name validation failures |
| [Mem0](https://github.com/mem0ai/mem0) (59.4k★) | [#5380](https://github.com/mem0ai/mem0/pull/5380) | Expose Qdrant's `https` option so self-hosted HTTP clusters can use API-key auth without forcing TLS client mode |
| [Mem0](https://github.com/mem0ai/mem0) (59.4k★) | [#5383](https://github.com/mem0ai/mem0/pull/5383) | Skip OpenClaw runtime setup during CLI metadata registration so plugin discovery does not double-register runtime side effects |
| [Agno](https://github.com/agno-agi/agno) (40.8k★) | [#8131](https://github.com/agno-agi/agno/pull/8131) | Preserve non-sentinel tool argument whitespace while keeping string-to-None/True/False normalization for exact sentinels |
| [GitHub MCP Server](https://github.com/github/github-mcp-server) (31.0k★) | [#2514](https://github.com/github/github-mcp-server/pull/2514) | Support team reviewers in pull-request review requests by resolving team slugs into GitHub review subjects instead of dropping them |
| [GitHub MCP Server](https://github.com/github/github-mcp-server) (31.0k★) | [#2612](https://github.com/github/github-mcp-server/pull/2612) | Hide write-side UI resources when the MCP server runs read-only, while keeping safe read-only resources registered |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (27.2k★) | [#1786](https://github.com/agentscope-ai/agentscope/pull/1786) | Preserve caller-provided Redis session ids on create so later get, update, and list operations address the same session instead of a generated UUID |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (27.2k★) | [#1815](https://github.com/agentscope-ai/agentscope/pull/1815) | Inherit leader permission rules in team runs so delegated agents keep the same workspace and file access constraints as the leader |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (27.2k★) | [#1823](https://github.com/agentscope-ai/agentscope/pull/1823) | Add workspace roots to permission context so chat runs authorize files against the actual agent-visible workspace |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (27.2k★) | [#1734](https://github.com/agentscope-ai/agentscope/pull/1734) | Expire Redis message lists by refreshing TTL on append and streaming replace writes, so configured storage TTL actually bounds chat history |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (27.2k★) | [#1774](https://github.com/agentscope-ai/agentscope/pull/1774) | Forward explicitly configured Qwen `thinking_enable` into OpenAI-compatible `extra_body` without polluting normal OpenAI requests |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (27.2k★) | [#1822](https://github.com/agentscope-ai/agentscope/pull/1822) | Add a cwd option to the built-in Bash tool so shell commands can run in the intended workspace directory |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (27.2k★) | [#1732](https://github.com/agentscope-ai/agentscope/pull/1732) | Include skills from every active tool group so prompt instructions and the Skill viewer stay aligned with enabled tools |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (27.2k★) | [#1717](https://github.com/agentscope-ai/agentscope/pull/1717) | Hide Bash tool subprocess windows on Windows with `CREATE_NO_WINDOW`, while leaving non-Windows process creation unchanged |
| [Pydantic AI](https://github.com/pydantic/pydantic-ai) (18.0k★) | [#5694](https://github.com/pydantic/pydantic-ai/pull/5694) | Fix `MCPToolset(http_client=...)` with FastMCP by keeping `follow_redirects` out of caller-provided HTTP client factories |
| [Pydantic AI](https://github.com/pydantic/pydantic-ai) (18.0k★) | [#5474](https://github.com/pydantic/pydantic-ai/pull/5474) | Accept `providerExecuted` and `title` on Vercel AI dynamic-tool message parts so strict validation preserves provider metadata |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (14.4k★) | [#1735](https://github.com/ag-ui-protocol/ag-ui/pull/1735) | Avoid stale ADK session writes after human-in-the-loop tool calls |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (14.4k★) | [#1828](https://github.com/ag-ui-protocol/ag-ui/pull/1828) | Detect Strands' private session manager so AG-UI history replay respects active sessions instead of duplicating prior turns |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (14.4k★) | [#1889](https://github.com/ag-ui-protocol/ag-ui/pull/1889) | Collect output-schema agents when building ADK workflow graphs so structured-output agent nodes are not dropped |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (14.4k★) | [#1826](https://github.com/ag-ui-protocol/ag-ui/pull/1826) | Forward LangGraph runtime context through tool kwargs so graph tools keep caller-supplied execution context |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (14.4k★) | [#1829](https://github.com/ag-ui-protocol/ag-ui/pull/1829) | Close LangGraph text messages before tool-call chunks so text-to-tool transitions keep both message and tool events |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (14.4k★) | [#1832](https://github.com/ag-ui-protocol/ag-ui/pull/1832) | Preserve AG-UI input metadata when LangGraph converts text and media blocks into LangChain multimodal content |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (14.4k★) | [#1890](https://github.com/ag-ui-protocol/ag-ui/pull/1890) | Cache ADK session reads within one execution so remote session services are not fetched repeatedly before each agent run |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (14.4k★) | [#1769](https://github.com/ag-ui-protocol/ag-ui/pull/1769) | Make proto generation cross-platform: replace Unix-only `mkdir -p` with a Node script and Windows `.CMD` plugin shim |
| [OpenHarness](https://github.com/HKUDS/OpenHarness) (14.1k★) | [#185](https://github.com/HKUDS/OpenHarness/pull/185) | TUI tab-completion: fix cursor jump, strip trailing space, accept `/quit` alias |
| [Pipecat](https://github.com/pipecat-ai/pipecat) (13.0k★) | [#4553](https://github.com/pipecat-ai/pipecat/pull/4553) | Serialize interruption frames through protobuf transports so realtime voice-agent interruptions survive transport hops |
| [LiveKit Agents](https://github.com/livekit/agents) (11.1k★) | [#5820](https://github.com/livekit/agents/pull/5820) | Recreate Anthropic streaming requests on retry so transient stream creation failures do not re-await the same coroutine |
| [LiveKit Agents](https://github.com/livekit/agents) (11.1k★) | [#5864](https://github.com/livekit/agents/pull/5864) | Surface Soniox STT server errors instead of treating failed streams as empty transcripts |
| [LiveKit Agents](https://github.com/livekit/agents) (11.1k★) | [#5994](https://github.com/livekit/agents/pull/5994) | Handle OpenAI-compatible realtime status details returned as strings so incomplete responses do not crash logging |
| [LiveKit Agents](https://github.com/livekit/agents) (11.1k★) | [#5872](https://github.com/livekit/agents/pull/5872) | Map ElevenLabs server-VAD committed transcripts to `END_OF_SPEECH` so realtime turns close without requiring manual empty commits |
| [LiveKit Agents](https://github.com/livekit/agents) (11.1k★) | [#5976](https://github.com/livekit/agents/pull/5976) | Preserve request timeouts when callers provide custom Google HTTP options, without mutating the caller-owned options object |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.3k★) | [#2340](https://github.com/strands-agents/harness-sdk/pull/2340) | Keep concurrent tool results in request order so parallel tool execution does not scramble model-visible outputs |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.3k★) | [#2353](https://github.com/strands-agents/harness-sdk/pull/2353) | Handle Gemini safety-blocked metadata by defaulting missing usage counts and mapping safety stops to guardrail intervention |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.3k★) | [#2354](https://github.com/strands-agents/harness-sdk/pull/2354) | Read vLLM `delta.reasoning` chunks in OpenAI-compatible streams so reasoning output survives provider conversion |
| [ClawTeam](https://github.com/HKUDS/ClawTeam) (5.3k★) | [#1](https://github.com/HKUDS/ClawTeam/pull/1) | First PR: 122 tests, CI, team templates, config bugfixes, task duration tracking |
| [ClawTeam](https://github.com/HKUDS/ClawTeam) (5.3k★) | [#40](https://github.com/HKUDS/ClawTeam/pull/40) | Pluggable TaskStore: extract task persistence into swappable backend abstraction |
| [ClawTeam](https://github.com/HKUDS/ClawTeam) (5.3k★) | [#32](https://github.com/HKUDS/ClawTeam/pull/32) | Gemini CLI support: spawn, permissions, prompt injection for both backends |
| [ClawTeam](https://github.com/HKUDS/ClawTeam) (5.3k★) | [#36](https://github.com/HKUDS/ClawTeam/pull/36) | Kimi CLI support: spawn backend, permission handling, 3 new test cases |
| [MCP Go SDK](https://github.com/modelcontextprotocol/go-sdk) (4.7k★) | [#962](https://github.com/modelcontextprotocol/go-sdk/pull/962) | Reject duplicate `initialize` requests so MCP sessions keep protocol state consistent after initialization |
| [MCP Go SDK](https://github.com/modelcontextprotocol/go-sdk) (4.7k★) | [#981](https://github.com/modelcontextprotocol/go-sdk/pull/981) | Add `Implementation.description` metadata while keeping empty descriptions out of serialized MCP payloads |
| [EvalScope](https://github.com/modelscope/evalscope) (3.0k★) | [#1381](https://github.com/modelscope/evalscope/pull/1381) | Read SciCode assistant answers from OpenAI-style text content blocks so scorer prompts receive the generated answer instead of an empty field |
| [OpenHands SDK](https://github.com/OpenHands/software-agent-sdk) (841★) | [#3248](https://github.com/OpenHands/software-agent-sdk/pull/3248) | Serialize LiteLLM `modify_params` updates with an RLock so concurrent completions do not leak global parameter state |
| [OpenHands SDK](https://github.com/OpenHands/software-agent-sdk) (841★) | [#3247](https://github.com/OpenHands/software-agent-sdk/pull/3247) | Validate git workspaces with `git rev-parse --git-dir` so broken nested repos do not crash `/api/git/changes` |
| [OpenHands SDK](https://github.com/OpenHands/software-agent-sdk) (841★) | [#3225](https://github.com/OpenHands/software-agent-sdk/pull/3225) | Write remote completion logs as UTF-8 so non-ASCII output survives local replay and debugging |

#### Applied AI / RAG / observability

| Project | PR | What I Fixed |
|---------|:--:|-------------|
| [RAGFlow](https://github.com/infiniflow/ragflow) (83.6k★) | [#15691](https://github.com/infiniflow/ragflow/pull/15691) | Skip empty agent switch conditions so blank branch guards do not crash or block valid downstream agent flows |
| [RAGFlow](https://github.com/infiniflow/ragflow) (83.6k★) | [#15696](https://github.com/infiniflow/ragflow/pull/15696) | Keep the strongest PageRank score for repeated n-hop GraphRAG edges instead of letting path order overwrite ranking |
| [RAGFlow](https://github.com/infiniflow/ragflow) (83.6k★) | [#15601](https://github.com/infiniflow/ragflow/pull/15601) | Fall back when Docling native parsing returns no chunks so documents still produce usable content instead of empty parse results |
| [LightRAG](https://github.com/HKUDS/LightRAG) (36.9k★) | [#2796](https://github.com/HKUDS/LightRAG/pull/2796) | Fix `None` file_path propagating as `unknown_source`: fill gaps left by #2793 |
| [LightRAG](https://github.com/HKUDS/LightRAG) (36.9k★) | [#3206](https://github.com/HKUDS/LightRAG/pull/3206) | Honor PostgreSQL `search_path` in table-existence checks so non-public schemas are detected before migrations or table creation |
| [LightRAG](https://github.com/HKUDS/LightRAG) (36.9k★) | [#3031](https://github.com/HKUDS/LightRAG/pull/3031) | Extract Docling async markdown results from the response envelope so RAG chunks contain clean document text |
| [LightRAG](https://github.com/HKUDS/LightRAG) (36.9k★) | [#3123](https://github.com/HKUDS/LightRAG/pull/3123) | Sync API documentation colors with the dark theme so endpoint examples stay readable in dark mode |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13637](https://github.com/Arize-ai/phoenix/pull/13637) | Wait for in-memory SQLite schema initialization before serving Phoenix so startup races do not hit missing tables |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13245](https://github.com/Arize-ai/phoenix/pull/13245) | Keep the generative model fetch cursor monotonic so lower-id updates cannot make later polling skip newer model changes |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13210](https://github.com/Arize-ai/phoenix/pull/13210) | Return NotFound-style errors for invalid GraphQL node ids instead of leaking decoder failures to clients |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13139](https://github.com/Arize-ai/phoenix/pull/13139) | Surface playground validation errors instead of returning empty subscription payloads |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13641](https://github.com/Arize-ai/phoenix/pull/13641) | Expire prompt tool diffs on provider change so PXI prompt editing does not carry stale tool-change state across providers |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13242](https://github.com/Arize-ai/phoenix/pull/13242) | Pass Anthropic computer-use beta headers for raw computer tool definitions in playground streaming and non-streaming calls |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13261](https://github.com/Arize-ai/phoenix/pull/13261) | Refresh span annotation notes after create so the UI shows newly added notes without a manual reload |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13614](https://github.com/Arize-ai/phoenix/pull/13614) | Refresh the prompts table while users stay on the page so newly created or updated prompts appear without a manual reload |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13653](https://github.com/Arize-ai/phoenix/pull/13653) | Focus the PXI input when the agent panel opens so keyboard-first agent workflows can start without an extra click |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13636](https://github.com/Arize-ai/phoenix/pull/13636) | Update PXI system prompt guidance to point at the current server-side Jinja templates and capability wiring instead of stale browser-side paths |
| [Graphiti](https://github.com/getzep/graphiti) (27.8k★) | [#1531](https://github.com/getzep/graphiti/pull/1531) | Strip embedded NUL bytes from FalkorDB query parameters so one malformed document string cannot crash bulk graph writes |

#### Recommender systems

| Project | PR | What I Fixed |
|---------|:--:|-------------|
| [Microsoft Recommenders](https://github.com/recommenders-team/recommenders) (21.8k★) | [#2345](https://github.com/recommenders-team/recommenders/pull/2345) | Query GPU memory through PyTorch first and keep numba as a fallback so GPU discovery does not fail on unavailable CUDA contexts |
| [Microsoft Recommenders](https://github.com/recommenders-team/recommenders) (21.8k★) | [#2322](https://github.com/recommenders-team/recommenders/pull/2322) | Honor benchmark recommendation-count args so evaluation scripts generate the requested top-k results |

### LinkedIn: https://www.linkedin.com/in/yufenghe

---

## Hi，我是何宇峰 👋

AI Agent 研究员 & 工程师 | 曾任 [Moonshot AI](https://www.moonshot.ai/) (Kimi) | 港大计算机硕士 | 上海全球AI大赛冠军 | 三次获ACM-ICPC银牌 | 曾在百度、脉脉、快手的AI 研发岗实习

- 200+ 个上游 PR 已 merged，其中 vLLM（9 个）、Mooncake（24 个）、Qwen Code（51 个）、Microsoft Agent Framework（20 个）、AstrBot（30 个）、Google ADK（10 个）、Inspect AI（18 个）、Hugging Face Transformers（1 个）、PyTorch（3 个）。
- 代表性公开项目（star 100+）：CoreCoder、FindJobs-Agent、RepoWiki、ContractGuard。

### 项目

| 方向 | 项目 | Stars | 简介 |
|------|------|:-----:|------|
| Coding agents / 评测 | [CoreCoder](https://github.com/he-yufeng/CoreCoder) | 1.5k+ | Claude Code 51万行源码 → 1400行 Python 核心重写，支持任意大模型，附 7 篇架构导读。 |
| 应用型 Agent | [FindJobs-Agent](https://github.com/he-yufeng/FindJobs-Agent) | 200+ | LLM 求职工具箱：技能差距分析、模拟面试、简历优化和岗位结构化。 |
| 代码库地图 | [RepoWiki](https://github.com/he-yufeng/RepoWiki) | 200+ | 开源 DeepWiki 替代品：CLI 或浏览器生成仓库 wiki，PageRank 文件排名、Mermaid 架构图、阅读指南。 |
| 应用型 Agent | [ContractGuard](https://github.com/he-yufeng/ContractGuard) | 100+ | AI 合同审查 Agent，签字前帮你找红旗条款、不公平约定和缺失保护。 |
| 代码库地图 | [GitSense](https://github.com/he-yufeng/GitSense) | 100+ | AI 开源贡献发现器 + 仓库雷达：找匹配 issue，也评估 PR 合入友好度。 |
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

#### AI infra / 模型系统

| 项目 | PR | 修了啥 |
|------|:--:|--------|
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#37884](https://github.com/vllm-project/vllm/pull/37884) | 修复 RoBERTa position_ids 原地累积溢出：BGE-M3 约 4000 请求后 CUDA graph padding crash |
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#40789](https://github.com/vllm-project/vllm/pull/40789) | 修复 V1 ubatch wrapper 不支持 tuple model outputs：DBO / speculative decoding 不再因 tuple 返回值崩溃 |
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#44821](https://github.com/vllm-project/vllm/pull/44821) | 给 DeepSeek V4 MTP projection layers 补 prefix，让 compressed-tensors 加载 draft model 时能匹配 artifact 侧 target / ignore 规则 |
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#43243](https://github.com/vllm-project/vllm/pull/43243) | 先按 JSON 解析 Qwen3 XML tool-call 参数，让 `null` / `false` 等 JSON literal 在 streaming tool parser 中稳定保留 |
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#37727](https://github.com/vllm-project/vllm/pull/37727) | 修复 Responses API 的 `instructions` 通过 `previous_response_id` 链泄漏到后续轮次 |
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#42679](https://github.com/vllm-project/vllm/pull/42679) | 保护 flash-attn rotary 导入路径，让 FA4 环境缺少 `flash_attn.ops.triton.rotary` 时稳定回退而不是构造 rotary 层时崩溃 |
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#37699](https://github.com/vllm-project/vllm/pull/37699) | 修复 weight offloading 忽略 `VLLM_WEIGHT_OFFLOADING_DISABLE_PIN_MEMORY` 环境变量 |
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#37301](https://github.com/vllm-project/vllm/pull/37301) | 修复 base64 JPEG 视频帧返回空 metadata：补充帧数、fps、时长 |
| [vLLM](https://github.com/vllm-project/vllm) (86.1k★) | [#38732](https://github.com/vllm-project/vllm/pull/38732) | 修复 bench_serve 流式响应拆分多字节 UTF-8 字符导致 decode 崩溃 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#1629](https://github.com/kvcache-ai/Mooncake/pull/1629) | GB200 MNNVL EP hang：`cudaMalloc` → `cuMemCreate(FABRIC)` + `cuMemMap` 跨节点 NVLink 通信 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#2570](https://github.com/kvcache-ai/Mooncake/pull/2570) | 修复 `BatchOffload` 处理 >4 GiB 对象时的整数溢出：用 `uint64_t` 累加各 slice 大小，并拒绝超过 `uint32_t` 记录 `value_len` 的对象，而不是静默截断 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#2610](https://github.com/kvcache-ai/Mooncake/pull/2610) | 恢复 `RdmaTransport::submitTransfer` 里的 `task.request` 关联：重构时漏掉了每个 task 的 `request` 指针赋值，导致下游拿到 null，status/重试/计费回读全部失效 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#1728](https://github.com/kvcache-ai/Mooncake/pull/1728) | Hard pin 驱逐保护：模型权重永不被驱逐，const 字段 + BatchEvict 跳过 + 向后兼容序列化 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#1719](https://github.com/kvcache-ai/Mooncake/pull/1719) | 新增 `ObjectDataType` 元数据分类：KV cache、weights、tensors 等对象类型可在 metadata、snapshot 和 Python binding 中稳定传递 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#1831](https://github.com/kvcache-ai/Mooncake/pull/1831) | TENT NVLink IPC 修复：sub-allocated GPU tensor 使用 base pointer，将 #1622 修复移植到 TENT 路径 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#1644](https://github.com/kvcache-ai/Mooncake/pull/1644) | MNNVL warmup hang：跳过 fabric 连接节点的冗余握手 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#1825](https://github.com/kvcache-ai/Mooncake/pull/1825) | 修复 `P2PClientService::Put` 静默吞掉写入错误：传播实际错误码给调用方 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#2402](https://github.com/kvcache-ai/Mooncake/pull/2402) | Python buddy allocator backing buffer 分配失败时直接拒绝，避免把 null raw buffer 放进 managed slab |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#2403](https://github.com/kvcache-ai/Mooncake/pull/2403) | 清理失败的 io_uring sub-batch 初始化状态，避免部分初始化失败的 transfer batch 把坏状态带入后续 setup |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#2311](https://github.com/kvcache-ai/Mooncake/pull/2311) | 让 HTTP metadata server 对相同 `rpc_meta` 重复发布保持幂等，同时继续拒绝内容变化的重复写入 |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) (5.8k★) | [#1626](https://github.com/kvcache-ai/Mooncake/pull/1626) | 修复非内存副本的错误日志刷屏 |
| [Transformers](https://github.com/huggingface/transformers) (162.5k★) | [#44710](https://github.com/huggingface/transformers/pull/44710) | 修复 `AutoProcessor.from_pretrained` 静默丢弃 hub kwargs（`revision`、`token` 等） |
| [PyTorch](https://github.com/pytorch/pytorch) (101.8k★) | [#176100](https://github.com/pytorch/pytorch/pull/176100) | 修复 Inductor codegen 中用户自定义 Triton kernel 的名称修饰，避免不同 kernel 在生成代码里命名冲突（PR 显示 Closed，经 pytorchmergebot 合入） |
| [PyTorch](https://github.com/pytorch/pytorch) (101.8k★) | [#187643](https://github.com/pytorch/pytorch/pull/187643) | 修复 `stale_issues` workflow 的 `parse_older_than` 在非闰年崩溃：朴素的 2 月 29 日偏移会抛 `ValueError`（PR 显示 Closed，经 pytorchmergebot 合入） |
| [PyTorch](https://github.com/pytorch/pytorch) (101.8k★) | [#187262](https://github.com/pytorch/pytorch/pull/187262) | 移除过时的 `setuptools` 版本上限，让构建解析到当前工具链而不是被钉在旧版本（PR 显示 Closed，经 pytorchmergebot 合入） |
| [LiteLLM](https://github.com/BerriAI/litellm) (51.4k★) | [#26401](https://github.com/BerriAI/litellm/pull/26401) | 修复 `LITELLM_LOG=INFO` 漏设 `verbose_logger`：proxy INFO 日志不再静默丢失 |
| [SGLang](https://github.com/sgl-project/sglang) (30.2k★) | [#20739](https://github.com/sgl-project/sglang/pull/20739) | 修复 hybrid_linear_attn_backend 与 ngram 投机采样同时使用时崩溃 |
| [verl](https://github.com/verl-project/verl) (22.4k★) | [#6620](https://github.com/verl-project/verl/pull/6620) | 按 data-parallel 和 tensor-parallel rank 计算 colocated vLLM 权重同步 ZMQ socket rank，避免多个 DP worker 连接到同一 receiver |
| [Triton](https://github.com/triton-lang/triton) (19.7k★) | [#9613](https://github.com/triton-lang/triton/pull/9613) | 修复 AxisInfo 正确性：有符号常量、未知 shift 和 shift UB 都保守处理 |
| [TRL](https://github.com/huggingface/trl) (18.8k★) | [#6054](https://github.com/huggingface/trl/pull/6054) | SFT 准备阶段拒绝已转换过的数据集，让配置错误的训练快速失败，而不是静默产出错误的训练 batch |
| [LMCache](https://github.com/LMCache/LMCache) (9.8k★) | [#3245](https://github.com/LMCache/LMCache/pull/3245) | 在 MP store/retrieve 请求期间保留 producer 侧 CUDA IPC event，避免 daemon 通过已回收 event handle 恢复时报 invalid argument |
| [LMCache](https://github.com/LMCache/LMCache) (9.8k★) | [#3282](https://github.com/LMCache/LMCache/pull/3282) | 支持 MP KV transfer 中的 HND GPU KV 格式，让不同 KV tensor layout 能被正确处理 |
| [FlashInfer](https://github.com/flashinfer-ai/flashinfer) (5.9k★) | [#2756](https://github.com/flashinfer-ai/flashinfer/pull/2756) | 修复 autotuner 在输入 tensor 为 `None` 时崩溃（fixes #2749） |
| [FlashInfer](https://github.com/flashinfer-ai/flashinfer) (5.9k★) | [#2772](https://github.com/flashinfer-ai/flashinfer/pull/2772) | 修复编译错误：CUTLASS 头文件缺少 `<optional>` include 导致 `std::optional` 未定义 |
| [Google Gen AI SDK](https://github.com/googleapis/python-genai) (3.8k★) | [#2564](https://github.com/googleapis/python-genai/pull/2564) | 让 Live Music API key 不再进入 websocket URL query，改由请求 header 承载，避免密钥出现在日志和代理路径里 |

#### Agent 框架 / 协议 / 评测

| 项目 | PR | 修了啥 |
|------|:--:|--------|
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5036](https://github.com/QwenLM/qwen-code/pull/5036) | 检测到重复工具调用循环后真正硬停止，避免 agent 继续执行同一个已卡住的动作 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5020](https://github.com/QwenLM/qwen-code/pull/5020) | 取消请求后丢弃残留 tool calls，避免中止轮次把过期工具调用泄漏到下一次 provider payload |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4622](https://github.com/QwenLM/qwen-code/pull/4622) | 保持 assistant tool calls 和 tool results 相邻，避免修复后的消息历史被 OpenAI-compatible provider 拒绝 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5071](https://github.com/QwenLM/qwen-code/pull/5071) | 流式输出结束后仍提交已完成的快速 tool results，避免模型流尾部竞态把工具结果留在本地队列 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4970](https://github.com/QwenLM/qwen-code/pull/4970) | 稳定 truncated tool retry key，让修复后的 tool call 在重试时保持确定性身份，不再因 key 漂移重复或错配 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5058](https://github.com/QwenLM/qwen-code/pull/5058) | 避免 stale tool schema recall，让 memory warning 不再把过期工具名带回后续规划轮次 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5062](https://github.com/QwenLM/qwen-code/pull/5062) | 跨 agent 轮次保留 token escalation 上下文，避免 delegated run 每轮都从容量不足的模型重新开始 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4828](https://github.com/QwenLM/qwen-code/pull/4828) | 认证刷新后保留用户配置的共享 `baseUrl`，避免同模型刷新把 endpoint 回退成 provider 默认值 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4829](https://github.com/QwenLM/qwen-code/pull/4829) | 给 Qwen OAuth refresh 增加超时，避免刷新端点卡住时 CLI 一直挂在认证恢复路径 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4607](https://github.com/QwenLM/qwen-code/pull/4607) | 修复 IDE proxy 请求：让 `fetch` 和 `EnvHttpProxyAgent` 保持在同一个 bundled `undici` 模块路径上 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4716](https://github.com/QwenLM/qwen-code/pull/4716) | 让 `/bug`、`/docs` 和 `/insight` 的浏览器打开路径复用安全 launcher，避免 headless 环境因直接 `open` 崩溃 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4596](https://github.com/QwenLM/qwen-code/pull/4596) | 仓库爬取时递归读取已跟踪 Git submodule，让 coding agent 上下文包含子模块内部文件 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5115](https://github.com/QwenLM/qwen-code/pull/5115) | team 功能关闭时隐藏 teammate 专属的 agent 名称参数；旧 prompt 仍传入名称时回退到 one-shot subagent，而不是直接失败 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5070](https://github.com/QwenLM/qwen-code/pull/5070) | 焦点导航时忽略已过期 live agents，避免 stale background-agent 行抢走键盘焦点 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5061](https://github.com/QwenLM/qwen-code/pull/5061) | 保留 background agent 启动参数，让 delegated CLI run 继续使用用户指定的执行模式 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4715](https://github.com/QwenLM/qwen-code/pull/4715) | 让 managed auto-memory 遵守运行时输出目录，同时保留显式 memory 目录覆盖的优先级 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4717](https://github.com/QwenLM/qwen-code/pull/4717) | 将 copy、arena、ACP snapshot 等退出路径的深拷贝改成浅层只读历史访问，同时保留 restore 写回路径的防御性克隆 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5043](https://github.com/QwenLM/qwen-code/pull/5043) | 让 grep 结果满足 prior-read 检查，已验证的搜索上下文不再被迫重复读取文件 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4673](https://github.com/QwenLM/qwen-code/pull/4673) | 修复顶层 `--list-extensions` / `-l`：按文档打印扩展列表，并在 sandbox、auth、TUI 启动前退出 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4632](https://github.com/QwenLM/qwen-code/pull/4632) | 强化 context error 文本抽取，让嵌套或非字符串错误 payload 也能暴露有用诊断信息 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5077](https://github.com/QwenLM/qwen-code/pull/5077) | permission gate 失败时展示完整计划，让用户能检查被拦截的 agent 意图 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5073](https://github.com/QwenLM/qwen-code/pull/5073) | 上下文指令文件超过预算时主动告警，避免仓库级 guidance 静默挤占任务上下文 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4963](https://github.com/QwenLM/qwen-code/pull/4963) | 默认启用 fork subagents，让 delegated work 能在隔离分支中运行而不用手动开启 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4600](https://github.com/QwenLM/qwen-code/pull/4600) | 区分 TUI 中 AUTO 与 AUTO_EDIT approval-mode 指示器：共享样式、本地化 key 和可视化证据一起补齐 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4738](https://github.com/QwenLM/qwen-code/pull/4738) | 复制 CLI 可见输出时跳过隐藏 thought 片段，让剪贴板内容和用户实际看到的一致 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4639](https://github.com/QwenLM/qwen-code/pull/4639) | 移除已停用的 Qwen OAuth ACP 登录路径，避免用户被引导到失效认证方式 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4636](https://github.com/QwenLM/qwen-code/pull/4636) | 将用户指定的输出语言同步到 side queries，让辅助回答也遵守主响应的语言约束 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#4635](https://github.com/QwenLM/qwen-code/pull/4635) | 在 CLI todo 视图中隐藏已完成 sticky todos，让持久任务提示只聚焦剩余工作 |
| [Qwen Code](https://github.com/QwenLM/qwen-code) (25.5k★) | [#5072](https://github.com/QwenLM/qwen-code/pull/5072) | 稳定 simple MCP 集成检查，避免服务就绪时序让跨进程协议测试偶发失败 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5462](https://github.com/microsoft/agent-framework/pull/5462) | 修复 `background=True` + tools 无限 retrieve loop：清掉已完成的 continuation 状态，让 tool results 正常提交 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5773](https://github.com/microsoft/agent-framework/pull/5773) | 把同步 Python 工具调用移出事件循环执行，避免阻塞型工具冻结并发 agent 任务 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#6210](https://github.com/microsoft/agent-framework/pull/6210) | reasoning payload 被剥离时同步丢弃 hosted MCP tool-call 历史，避免 stateless OpenAI replay 发送孤立 MCP 调用 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#6132](https://github.com/microsoft/agent-framework/pull/6132) | 按 session id 过滤 filesystem checkpoint index，避免 reopen store 后返回其它 workflow session 的 checkpoint |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5904](https://github.com/microsoft/agent-framework/pull/5904) | AG-UI thread id 下继续使用 ChatClientAgent 本地历史 provider，避免把 session history 误判为服务端模型历史 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#6208](https://github.com/microsoft/agent-framework/pull/6208) | 修复声明式 `Foreach` 对 PowerFx record 行的取值，避免多字段 table row 在循环中被折叠 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5861](https://github.com/microsoft/agent-framework/pull/5861) | 修复 Foundry handoff 参数序列化，delegated agent 调用不再丢失结构化参数 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5808](https://github.com/microsoft/agent-framework/pull/5808) | 修复 handoff message role 原地修改：重试复用消息时不再把角色变更泄漏到后续流程 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5784](https://github.com/microsoft/agent-framework/pull/5784) | 转换历史消息时跳过孤立的 Anthropic thinking signature，避免 replay 时携带无效的 standalone signature |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5778](https://github.com/microsoft/agent-framework/pull/5778) | 补齐 Magentic protocol 的 chat/reset message 声明，避免 orchestrator 反序列化未知类型失败 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5800](https://github.com/microsoft/agent-framework/pull/5800) | 修复 AG-UI tool result message id 冲突：provider 省略 update id 时仍能生成独立 fallback id |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5801](https://github.com/microsoft/agent-framework/pull/5801) | 按 call id 合并 code interpreter streaming 历史片段，让最终存储的代码和结果完整保留且不重复记录 delta |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5974](https://github.com/microsoft/agent-framework/pull/5974) | 让 Foundry agent eval 映射保留工具定义，评测运行能正常调用代码定义的 tools |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#6037](https://github.com/microsoft/agent-framework/pull/6037) | 保留 Foundry citation `get_url` 元数据，让检索引用链接经过 response conversion 后仍能出现在 chat response 中 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#6040](https://github.com/microsoft/agent-framework/pull/6040) | 转发 Foundry agent `default_headers` 到 OpenAI client 创建路径，让自定义认证和路由 headers 在 agent 初始化后仍然保留 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5815](https://github.com/microsoft/agent-framework/pull/5815) | 转发 MCP `tools/list` 元数据到 `call_tool` instrumentation，让 trace 保留工具注解 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5799](https://github.com/microsoft/agent-framework/pull/5799) | 补齐 Handoff workflow 的 name/description 元数据传递，让 builder 和 hosting 注册都能命名工作流 |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) (11.6k★) | [#5976](https://github.com/microsoft/agent-framework/pull/5976) | 修复 sequential workflow 示例输出，让非 streaming 结果展示所有参与 agent 的回复 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#6474](https://github.com/AstrBotDevs/AstrBot/pull/6474) | 修复 SQLite 并发写入 `database is locked`，添加 busy timeout |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#6596](https://github.com/AstrBotDevs/AstrBot/pull/6596) | 多模态 token 计数：图片/音频/思考链对 context 压缩不可见的问题 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#7003](https://github.com/AstrBotDevs/AstrBot/pull/7003) | 修复 WebChat 长响应断连：SSE 心跳保活，context 压缩期间不再超时 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#6581](https://github.com/AstrBotDevs/AstrBot/pull/6581) | 修复截断器丢失唯一 user 消息导致智谱/Gemini 返回 400 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#7216](https://github.com/AstrBotDevs/AstrBot/pull/7216) | 修复 Gemini tool call 400：纯文本 tool result 包装为 Protobuf Struct |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#6313](https://github.com/AstrBotDevs/AstrBot/pull/6313) | 修复 OpenAI API 返回 `None` choices 导致崩溃 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#6551](https://github.com/AstrBotDevs/AstrBot/pull/6551) | 修复空 content 导致 Grok 400：content 为空时设为 None |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#7407](https://github.com/AstrBotDevs/AstrBot/pull/7407) | 修复 Gemini 原生搜索无 function tools 时 400：跳过 FunctionCallingConfig |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#7196](https://github.com/AstrBotDevs/AstrBot/pull/7196) | 修复 Gemini thinking parts 泄漏到用户可见的消息内容中 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#7758](https://github.com/AstrBotDevs/AstrBot/pull/7758) | 修复 OpenAI streaming 路径复用 empty-assistant 过滤：reasoning-only 历史不再让严格 provider 返回 400 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8089](https://github.com/AstrBotDevs/AstrBot/pull/8089) | 图片请求在主 provider 不支持视觉输入时自动切到 vision fallback provider |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8119](https://github.com/AstrBotDevs/AstrBot/pull/8119) | 修复 active reply 图片输入丢失：把图片组件转成 image URLs 传给 LLM，保留原有文本 prompt 行为 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8073](https://github.com/AstrBotDevs/AstrBot/pull/8073) | 修复纯图片/表情消息的知识库空 prompt：空白文本时跳过 KB 检索，避免 embedding API 400 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#6710](https://github.com/AstrBotDevs/AstrBot/pull/6710) | 修复 skills-like re-query 丢失图片描述：`extra_user_content_parts` 未传递 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8195](https://github.com/AstrBotDevs/AstrBot/pull/8195) | 修复空 LLM summary：压缩器在模型返回空摘要时保留原始历史，不再插入空 summary 占位 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#7537](https://github.com/AstrBotDevs/AstrBot/pull/7537) | 修复 Telegram media group 异常被 APScheduler 静默吞掉：try/except + EVENT_JOB_ERROR listener |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#7398](https://github.com/AstrBotDevs/AstrBot/pull/7398) | 修复 Telegram 流式模式下空文本 sendMessageDraft 导致 400 错误刷屏 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8175](https://github.com/AstrBotDevs/AstrBot/pull/8175) | 修复 WeChat OA 媒体发送失败仍上报成功：prepare/send 超时或失败时向调用方抛出明确错误 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#6656](https://github.com/AstrBotDevs/AstrBot/pull/6656) | 修复 `/stop` 后新消息仍被 follow-up 捕获的竞态条件 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8061](https://github.com/AstrBotDevs/AstrBot/pull/8061) | 修复 Discord 启动同步命令触发 daily create quota 时打断 bot 启动：只把配额错误降级为 warning，其它异常继续抛出 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#7217](https://github.com/AstrBotDevs/AstrBot/pull/7217) | 修复 qwen3-rerank 响应解析：兼容新旧百炼 API 格式 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8768](https://github.com/AstrBotDevs/AstrBot/pull/8768) | 清理 Lark platform id 后缀中的不可见空白，避免配置里的尾部空格破坏平台匹配 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8736](https://github.com/AstrBotDevs/AstrBot/pull/8736) | 保留 embedding API version suffix，避免带版本的 provider endpoint 被归一化成错误路径 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8255](https://github.com/AstrBotDevs/AstrBot/pull/8255) | 支持 RST / AsciiDoc 知识库上传：后端解析白名单和前端文件校验同步扩展，避免支持的文档格式被入口拦截 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8718](https://github.com/AstrBotDevs/AstrBot/pull/8718) | 避免多模态回复在引用文本和图片 metadata 同时存在时重复显示 quoted image caption |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8172](https://github.com/AstrBotDevs/AstrBot/pull/8172) | 修复 release 使用过期 dashboard dist 的问题：优先加载 bundled WebUI 资产，避免发版后仍展示旧前端 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#6527](https://github.com/AstrBotDevs/AstrBot/pull/6527) | 修复 LLM 工具选择：重写模糊的 Upload/Download 描述 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8750](https://github.com/AstrBotDevs/AstrBot/pull/8750) | 修复 changelog anchor 链接，dashboard release notes 能跳转到正确小节 |
| [AstrBot](https://github.com/AstrBotDevs/AstrBot) (35.3k★) | [#8388](https://github.com/AstrBotDevs/AstrBot/pull/8388) | 补齐插件详情页 sub-command 数量的 dashboard i18n，避免页面展示原始翻译 key |
| [Google ADK](https://github.com/google/adk-python) (20.3k★) | [#5698](https://github.com/google/adk-python/pull/5698) | 让 `final_response_match_v2` 在 criterion 选择开启时把 intermediate responses 纳入最终回答评判 |
| [Google ADK](https://github.com/google/adk-python) (20.3k★) | [#5918](https://github.com/google/adk-python/pull/5918) | 允许 builder assistant 内部特殊 app name 通过 CLI runner 校验，让 `adk web` 能打开该特殊 agent |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#3896](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3896) | 修复 filestore recovery append 模式：保留已恢复 message/tool-call 池，同时避免重复哈希旧片段 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#3982](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3982) | 保留 agent bridge 转换中的 OpenAI wrapped reasoning payload，避免 encrypted provider-native reasoning item 在 transcript 转换时丢失 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#3975](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3975) | 修复 role model override 合并配置：角色切换模型时保留调用侧 `GenerateConfig` 默认值，不再丢掉 max tokens / reasoning effort 等设置 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#4069](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4069) | 周期性 flush streamed score samples，让长时间评测在结束前也能持续落盘 score 记录 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#3924](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3924) | 让未知 `GenerateConfig` 字段提前报错，避免拼错的生成参数被静默忽略 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#3941](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3941) | 修复 Bedrock Nova `top_k` 路由：把采样控制传到 inference config，而不是被静默丢弃 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#3902](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3902) | 修复 OpenAI-compatible 响应里的 OpenRouter `reasoning_details`：解析为可读 reasoning 文本，而不是暴露 Python repr |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#3895](https://github.com/UKGovernmentBEIS/inspect_ai/pull/3895) | 修复 `TERM=dumb` 下终端宽度：尊重 `COLUMNS`，日志输出不再固定按 Rich 默认 80 列硬换行 |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) (2.3k★) | [#4090](https://github.com/UKGovernmentBEIS/inspect_ai/pull/4090) | 澄清 model-graded history prompt：`include_history=True` 和最终答案字段的位置与实际 scorer 行为保持一致 |
| [OpenClaw](https://github.com/openclaw/openclaw) (380.3k★) | [#41259](https://github.com/openclaw/openclaw/pull/41259) | 目录创建失败时向上传递错误，避免 memory `ensureDir` 静默失败后继续执行 |
| [OpenClaw](https://github.com/openclaw/openclaw) (380.3k★) | [#41271](https://github.com/openclaw/openclaw/pull/41271) | 认证配置解析失败时记录日志而非静默吞掉 |
| [OpenHands](https://github.com/OpenHands/OpenHands) (78.3k★) | [#14776](https://github.com/OpenHands/OpenHands/pull/14776) | 编辑 basic model 设置时保留自定义 LLM base URL，避免保存 profile 后静默回退到 provider 默认 endpoint |
| [Cline](https://github.com/cline/cline) (63.9k★) | [#11166](https://github.com/cline/cline/pull/11166) | open-tabs host RPC 不可用时仍保持文件搜索可用，并回退到系统 `rg`，避免搜索链路直接失效 |
| [Mem0](https://github.com/mem0ai/mem0) (59.4k★) | [#5416](https://github.com/mem0ai/mem0/pull/5416) | 修复 S3 Vectors entity index 命名，避免 agent memory 写入因 AWS index-name 校验失败 |
| [Mem0](https://github.com/mem0ai/mem0) (59.4k★) | [#5380](https://github.com/mem0ai/mem0/pull/5380) | 暴露 Qdrant `https` 配置，让自托管 HTTP Qdrant + API key 场景不再被迫走 TLS client 模式 |
| [Mem0](https://github.com/mem0ai/mem0) (59.4k★) | [#5383](https://github.com/mem0ai/mem0/pull/5383) | OpenClaw CLI metadata 注册时跳过 runtime setup，避免插件发现阶段重复注册运行时副作用 |
| [Agno](https://github.com/agno-agi/agno) (40.8k★) | [#8131](https://github.com/agno-agi/agno/pull/8131) | 保留非哨兵工具参数字符串里的空白，同时继续只对精确的 None / True / False 哨兵做归一化 |
| [GitHub MCP Server](https://github.com/github/github-mcp-server) (31.0k★) | [#2514](https://github.com/github/github-mcp-server/pull/2514) | 支持 PR review 请求里的 team reviewer，把 team slug 解析为 GitHub review subject，不再丢失团队 reviewer |
| [GitHub MCP Server](https://github.com/github/github-mcp-server) (31.0k★) | [#2612](https://github.com/github/github-mcp-server/pull/2612) | read-only 模式下隐藏会写入 GitHub 的 UI resources，同时保留安全的只读资源注册 |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (27.2k★) | [#1786](https://github.com/agentscope-ai/agentscope/pull/1786) | 创建 Redis session 时保留调用方提供的 session id，让后续 get、update 和 list 操作继续命中同一 session，而不是生成的新 UUID |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (27.2k★) | [#1815](https://github.com/agentscope-ai/agentscope/pull/1815) | team run 中继承 leader permission rules，让 delegated agents 继续遵守同一套 workspace / file access 约束 |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (27.2k★) | [#1823](https://github.com/agentscope-ai/agentscope/pull/1823) | 把 workspace root 加入 permission context，让 chat run 按 agent 实际可见的 workspace 做文件授权 |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (27.2k★) | [#1734](https://github.com/agentscope-ai/agentscope/pull/1734) | Redis message list 写入和 streaming replace 时刷新 TTL，让配置的 storage TTL 真正约束聊天历史保留时间 |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (27.2k★) | [#1774](https://github.com/agentscope-ai/agentscope/pull/1774) | 显式设置 Qwen `thinking_enable` 时转发到 OpenAI-compatible `extra_body`，同时不污染普通 OpenAI 请求 |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (27.2k★) | [#1822](https://github.com/agentscope-ai/agentscope/pull/1822) | 给内置 Bash tool 增加 cwd 选项，让 shell 命令能在指定 workspace 目录执行 |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (27.2k★) | [#1732](https://github.com/agentscope-ai/agentscope/pull/1732) | 汇总所有已启用 tool group 的 skills，让 prompt instructions 和 Skill viewer 与当前启用工具保持一致 |
| [AgentScope](https://github.com/agentscope-ai/agentscope) (27.2k★) | [#1717](https://github.com/agentscope-ai/agentscope/pull/1717) | Windows 上启动 Bash tool 子进程时使用 `CREATE_NO_WINDOW`，避免工具执行弹出控制台窗口 |
| [Pydantic AI](https://github.com/pydantic/pydantic-ai) (18.0k★) | [#5694](https://github.com/pydantic/pydantic-ai/pull/5694) | 修复 `MCPToolset(http_client=...)` 与 FastMCP 的兼容问题，避免把 `follow_redirects` 泄漏给调用方提供的 HTTP client factory |
| [Pydantic AI](https://github.com/pydantic/pydantic-ai) (18.0k★) | [#5474](https://github.com/pydantic/pydantic-ai/pull/5474) | 兼容 Vercel AI dynamic-tool 消息里的 `providerExecuted` 和 `title` 字段，保留 provider 元数据而不是被严格校验拒绝 |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (14.4k★) | [#1735](https://github.com/ag-ui-protocol/ag-ui/pull/1735) | 修复 HITL tool call 后 ADK session 可能被旧状态回写的问题 |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (14.4k★) | [#1828](https://github.com/ag-ui-protocol/ag-ui/pull/1828) | 识别 Strands 私有 `_session_manager`，让 AG-UI history replay 尊重活跃 session，避免重复回放旧轮次 |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (14.4k★) | [#1889](https://github.com/ag-ui-protocol/ag-ui/pull/1889) | 构建 ADK workflow graph 时收集 output_schema agents，避免结构化输出 agent 节点被遗漏 |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (14.4k★) | [#1826](https://github.com/ag-ui-protocol/ag-ui/pull/1826) | 将 LangGraph runtime context 透传到 tool kwargs，让 graph tools 保留调用方传入的执行上下文 |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (14.4k★) | [#1829](https://github.com/ag-ui-protocol/ag-ui/pull/1829) | LangGraph 流从文本切到 tool call 时先关闭当前文本消息，避免工具调用事件被前一段文本吞掉 |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (14.4k★) | [#1832](https://github.com/ag-ui-protocol/ag-ui/pull/1832) | LangGraph 转换文本和媒体 block 时保留 AG-UI `InputContent.metadata` |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (14.4k★) | [#1890](https://github.com/ag-ui-protocol/ag-ui/pull/1890) | 在一次 ADK execution 内缓存 session 读取，避免远端 session service 在 agent 运行前被重复拉取完整历史 |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) (14.4k★) | [#1769](https://github.com/ag-ui-protocol/ag-ui/pull/1769) | 将 proto generation 从 Unix-only `mkdir -p` 改为跨平台 Node 脚本，兼容 Windows `.CMD` plugin shim |
| [OpenHarness](https://github.com/HKUDS/OpenHarness) (14.1k★) | [#185](https://github.com/HKUDS/OpenHarness/pull/185) | TUI tab 补全三合一修复：光标跳回、去除尾部空格、接受 `/quit` 别名 |
| [Pipecat](https://github.com/pipecat-ai/pipecat) (13.0k★) | [#4553](https://github.com/pipecat-ai/pipecat/pull/4553) | 修复 protobuf transport 丢失 interruption frame：实时语音 agent 的打断事件跨传输后仍能保留 |
| [LiveKit Agents](https://github.com/livekit/agents) (11.1k★) | [#5820](https://github.com/livekit/agents/pull/5820) | 修复 Anthropic streaming retry：瞬时建流失败后重新创建 stream，不再重复 await 同一个 coroutine |
| [LiveKit Agents](https://github.com/livekit/agents) (11.1k★) | [#5864](https://github.com/livekit/agents/pull/5864) | 暴露 Soniox STT server error：流式识别失败时返回明确错误，不再被当成空 transcript |
| [LiveKit Agents](https://github.com/livekit/agents) (11.1k★) | [#5994](https://github.com/livekit/agents/pull/5994) | 兼容 OpenAI-compatible realtime 返回字符串 status details，避免 incomplete response 在日志路径崩溃 |
| [LiveKit Agents](https://github.com/livekit/agents) (11.1k★) | [#5872](https://github.com/livekit/agents/pull/5872) | 将 ElevenLabs server-VAD committed transcript 映射为 `END_OF_SPEECH`，让 realtime turn 不再依赖手动空 commit 才结束 |
| [LiveKit Agents](https://github.com/livekit/agents) (11.1k★) | [#5976](https://github.com/livekit/agents/pull/5976) | 调用方传入自定义 Google HTTP options 时仍保留请求 timeout，并避免原地修改调用方对象 |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.3k★) | [#2340](https://github.com/strands-agents/harness-sdk/pull/2340) | 保持并发 tool results 按请求顺序回填，避免并行工具执行把模型可见结果顺序打乱 |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.3k★) | [#2353](https://github.com/strands-agents/harness-sdk/pull/2353) | 处理 Gemini safety-blocked metadata：缺失 token 计数时安全归零，并把 safety stop 映射为 guardrail intervention |
| [Strands Agents SDK](https://github.com/strands-agents/harness-sdk) (6.3k★) | [#2354](https://github.com/strands-agents/harness-sdk/pull/2354) | 读取 OpenAI-compatible vLLM stream 里的 `delta.reasoning`，让 reasoning 输出经过 provider conversion 后不丢失 |
| [ClawTeam](https://github.com/HKUDS/ClawTeam) (5.3k★) | [#1](https://github.com/HKUDS/ClawTeam/pull/1) | 首个 PR：122 个测试、CI、团队模板、config 修复、任务耗时追踪 |
| [ClawTeam](https://github.com/HKUDS/ClawTeam) (5.3k★) | [#40](https://github.com/HKUDS/ClawTeam/pull/40) | 可插拔 TaskStore：将任务持久化抽取为可替换的后端抽象层 |
| [ClawTeam](https://github.com/HKUDS/ClawTeam) (5.3k★) | [#32](https://github.com/HKUDS/ClawTeam/pull/32) | Gemini CLI 支持：spawn、权限、prompt 注入双 backend 适配 |
| [ClawTeam](https://github.com/HKUDS/ClawTeam) (5.3k★) | [#36](https://github.com/HKUDS/ClawTeam/pull/36) | Kimi CLI 支持：spawn backend、权限处理、3 个新测试 |
| [MCP Go SDK](https://github.com/modelcontextprotocol/go-sdk) (4.7k★) | [#962](https://github.com/modelcontextprotocol/go-sdk/pull/962) | 拒绝重复 `initialize` 请求，让 MCP session 初始化后的协议状态保持一致 |
| [MCP Go SDK](https://github.com/modelcontextprotocol/go-sdk) (4.7k★) | [#981](https://github.com/modelcontextprotocol/go-sdk/pull/981) | 补齐 `Implementation.description` 元数据，同时让空描述继续不进入序列化后的 MCP payload |
| [EvalScope](https://github.com/modelscope/evalscope) (3.0k★) | [#1381](https://github.com/modelscope/evalscope/pull/1381) | 读取 SciCode 评测中的 OpenAI-style text content blocks，让 scorer prompt 拿到真实 assistant 答案而不是空字段 |
| [OpenHands SDK](https://github.com/OpenHands/software-agent-sdk) (841★) | [#3248](https://github.com/OpenHands/software-agent-sdk/pull/3248) | 用 RLock 串行化 LiteLLM `modify_params` 的保存、设置和恢复，避免并发 completion 泄漏全局参数状态 |
| [OpenHands SDK](https://github.com/OpenHands/software-agent-sdk) (841★) | [#3247](https://github.com/OpenHands/software-agent-sdk/pull/3247) | 用 `git rev-parse --git-dir` 验证 git workspace，避免坏的 nested repo 打崩 `/api/git/changes` |
| [OpenHands SDK](https://github.com/OpenHands/software-agent-sdk) (841★) | [#3225](https://github.com/OpenHands/software-agent-sdk/pull/3225) | 按 UTF-8 写入 remote completion 日志，避免中文和非 ASCII 输出在本地回放、排查时损坏 |

#### 应用型 AI / RAG / 可观测性

| 项目 | PR | 修了啥 |
|------|:--:|--------|
| [RAGFlow](https://github.com/infiniflow/ragflow) (83.6k★) | [#15691](https://github.com/infiniflow/ragflow/pull/15691) | 跳过空的 agent switch 条件，避免空分支判断让有效后续 agent 流程崩溃或卡住 |
| [RAGFlow](https://github.com/infiniflow/ragflow) (83.6k★) | [#15696](https://github.com/infiniflow/ragflow/pull/15696) | repeated n-hop GraphRAG edges 保留最强 PageRank 分数，避免路径顺序覆盖排序结果 |
| [RAGFlow](https://github.com/infiniflow/ragflow) (83.6k★) | [#15601](https://github.com/infiniflow/ragflow/pull/15601) | Docling native 解析没有产出 chunks 时自动降级，避免文档解析结果变成空内容 |
| [LightRAG](https://github.com/HKUDS/LightRAG) (36.9k★) | [#2796](https://github.com/HKUDS/LightRAG/pull/2796) | 修复 `None` file_path 传播为 `unknown_source`：补 #2793 遗漏的处理层 |
| [LightRAG](https://github.com/HKUDS/LightRAG) (36.9k★) | [#3206](https://github.com/HKUDS/LightRAG/pull/3206) | 让 PostgreSQL 表存在性检查尊重当前 `search_path`，避免非 public schema 下迁移或建表判断失真 |
| [LightRAG](https://github.com/HKUDS/LightRAG) (36.9k★) | [#3031](https://github.com/HKUDS/LightRAG/pull/3031) | 从 Docling 异步结果 envelope 中抽取 Markdown 正文，避免 RAG chunk 混入 JSON/base64 噪声 |
| [LightRAG](https://github.com/HKUDS/LightRAG) (36.9k★) | [#3123](https://github.com/HKUDS/LightRAG/pull/3123) | 同步 API 文档暗色主题配色，避免 endpoint 示例在 dark mode 下变得不可读 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13637](https://github.com/Arize-ai/phoenix/pull/13637) | 等待 in-memory SQLite schema 初始化完成再服务 Phoenix，避免启动竞态导致 missing table |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13245](https://github.com/Arize-ai/phoenix/pull/13245) | 修复 generative model fetch 游标回退：低 id 更新不会让后续轮询跳过更新的模型变更 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13210](https://github.com/Arize-ai/phoenix/pull/13210) | 修复非法 GraphQL node id 的错误处理：返回 NotFound 风格错误，而不是把 decoder failure 泄漏给客户端 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13139](https://github.com/Arize-ai/phoenix/pull/13139) | 修复 Playground 校验错误被吞掉的问题：失败时返回明确错误，而不是空 subscription payload |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13641](https://github.com/Arize-ai/phoenix/pull/13641) | provider 变化时让 prompt tool diff 过期，避免 PXI prompt 编辑跨 provider 携带旧工具差异状态 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13242](https://github.com/Arize-ai/phoenix/pull/13242) | 为 raw computer tool definitions 传递 Anthropic computer-use beta headers，覆盖 playground streaming 和非 streaming 调用 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13261](https://github.com/Arize-ai/phoenix/pull/13261) | 修复 span annotation note 新建后的刷新问题：创建成功后立即重新拉取列表，前端不再需要手动刷新才能看到新 note |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13614](https://github.com/Arize-ai/phoenix/pull/13614) | 修复 Prompts 表格停留页面时不会自动刷新的问题：新建或更新的 prompt 不再需要手动刷新才能出现 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13653](https://github.com/Arize-ai/phoenix/pull/13653) | PXI agent 面板打开时自动聚焦输入框，让键盘优先的 agent workflow 不再多一次点击 |
| [Phoenix](https://github.com/Arize-ai/phoenix) (10.3k★) | [#13636](https://github.com/Arize-ai/phoenix/pull/13636) | 更新 PXI system prompt 指南，指向当前 server-side Jinja 模板和 capability wiring，不再引用过期的 browser-side 路径 |
| [Graphiti](https://github.com/getzep/graphiti) (27.8k★) | [#1531](https://github.com/getzep/graphiti/pull/1531) | 递归清理 FalkorDB 查询参数里的 NUL 字节，避免单个异常文档字符串打断批量图写入 |

#### 推荐系统

| 项目 | PR | 修了啥 |
|------|:--:|--------|
| [Microsoft Recommenders](https://github.com/recommenders-team/recommenders) (21.8k★) | [#2345](https://github.com/recommenders-team/recommenders/pull/2345) | 优先通过 PyTorch 查询 GPU 显存，并保留 numba fallback，避免 CUDA context 不可用时 GPU discovery 直接失败 |
| [Microsoft Recommenders](https://github.com/recommenders-team/recommenders) (21.8k★) | [#2322](https://github.com/recommenders-team/recommenders/pull/2322) | 修复 benchmark 推荐数量参数不生效，让评测脚本按请求生成 top-k 结果 |

### 领英LinkedIn: https://www.linkedin.com/in/yufenghe
