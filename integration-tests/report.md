# Integration Test Report

## Submitter

- **Git user:** Shaowei Chen <swchen.tw@gmail.com>
- **OS user:** `swchen.tw`
- **Hostname:** `HomeMacBook-Air.local`
- **Local IP:** `172.20.10.14`
- **Captured at:** 2026-05-18T04:33:39Z

## Setup

**Expert:** `framework-base-expert, wifi-bora-base-expert, wifi-bora-memory-slim-expert`
**Agent:** `claude-code` | **Model:** `claude-sonnet-4-6` | **Mode:** `headless`
**Date:** 2026-05-18T04:33:39.176630+00:00
**Pass Rate:** **7/8** (88%)

**Install Command:**
```
python3 /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/scripts/setup.py --add /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/framework/framework-base-expert, wifi-bora-base-expert, wifi-bora-memory-slim-expert/expert.json
```

**Working Directory:** `/Users/swchen.tw/git/workspace_jarvis`

## Summary Table

### Basic Metrics

| # | Test Case | Status | Duration | Tokens | Session Cost | Verify Cost | Grand Total |
|---|-----------|--------|----------|--------|-------------|------------|------------|
| 1 | FW-005 feedback_report_flow_trigger | PASS | 102s | 444K | $0.31 | $0.00 | $0.31 |
| 2 | FW-001 skill_create_flow_trigger | PASS | 106s | 264K | $0.22 | $0.00 | $0.22 |
| 3 | FW-006 feedback_report_cross_session | PASS | 85s | 304K | $0.22 | $0.00 | $0.22 |
| 4 | FW-002 expert_create_flow_trigger | PASS | 166s | 342K | $0.22 | $0.00 | $0.22 |
| 5 | WB-001 hello_world_with_size_check | FAIL | 68s | 331K | $0.20 | $0.00 | $0.20 |
| 6 | MEM-004 cross_dependency_skill_access | PASS | 18s | 97K | $0.08 | $0.00 | $0.08 |
| 7 | MEM-003 lsp_tool_trigger | PASS | 91s | 270K | $0.19 | $0.00 | $0.19 |
| 8 | MEM-002 memslim_flow_trigger | PASS | 115s | 287K | $0.23 | $0.00 | $0.23 |
| | **Total** | **7/8** | **751s** | **2342K** | **$1.67** | **$0.00** | **$1.67** |

### Session Analysis KPI

| # | Test Case | K1 | K2 | K3 | K4 | K5 | S1 | S2 | S3 | S4 | S5 | S6 |
|---|-----------|----|----|----|----|----|----|----|----|----|----|----|
| 1 | FW-005 | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A |
| 2 | FW-001 | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A |
| 3 | FW-006 | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A |
| 4 | FW-002 | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A |
| 5 | WB-001 | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A |
| 6 | MEM-004 | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A |
| 7 | MEM-003 | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A |
| 8 | MEM-002 | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A |

### Token Efficiency

| # | Test Case | Effective | Wasted | Efficiency% |
|---|-----------|-----------|--------|------------|
| 1 | FW-005 | 444,090 | 0 | 100.0% |
| 2 | FW-001 | 264,494 | 0 | 100.0% |
| 3 | FW-006 | 304,169 | 0 | 100.0% |
| 4 | FW-002 | 342,681 | 0 | 100.0% |
| 5 | WB-001 | 331,941 | 0 | 100.0% |
| 6 | MEM-004 | 97,019 | 0 | 100.0% |
| 7 | MEM-003 | 270,972 | 0 | 100.0% |
| 8 | MEM-002 | 287,467 | 0 | 100.0% |

### Behavior Phases

| # | Test Case | understanding | designing | exploring | implementing | debugging | verifying |
|---|-----------|---|---|---|---|---|---|
| 1 | FW-005 | 0 (0%) | 0 (0%) | 0 (0%) | 18 (78%) | 0 (0%) | 5 (22%) |
| 2 | FW-001 | 1 (5%) | 0 (0%) | 8 (40%) | 6 (30%) | 0 (0%) | 5 (25%) |
| 3 | FW-006 | 2 (9%) | 0 (0%) | 0 (0%) | 20 (87%) | 0 (0%) | 1 (4%) |
| 4 | FW-002 | 2 (8%) | 0 (0%) | 5 (19%) | 15 (58%) | 0 (0%) | 4 (15%) |
| 5 | WB-001 | 3 (12%) | 0 (0%) | 3 (12%) | 20 (77%) | 0 (0%) | 0 (0%) |
| 6 | MEM-004 | 2 (29%) | 0 (0%) | 0 (0%) | 5 (71%) | 0 (0%) | 0 (0%) |
| 7 | MEM-003 | 2 (12%) | 0 (0%) | 2 (12%) | 12 (71%) | 0 (0%) | 1 (6%) |
| 8 | MEM-002 | 2 (8%) | 0 (0%) | 1 (4%) | 19 (79%) | 0 (0%) | 2 (8%) |

### NL Check Detail

## Per-Test Details

### FW-005 feedback_report_flow_trigger — PASS (102.0s)

**Command:**
```
claude -p 我有這個 skills framework-skill-create-flow 嗎？這個 skill 中提到要創建新的 skills 命名規則是什麼？

回答完後，請使用 framework-feedback-report-flow 幫我打包最新的 session 的 feedback。給 3 分，理由是「測試用途，驗證打包流程」。 --output-format stream-json --model claude-sonnet-4-6 --verbose --dangerously-skip-permissions
```

**Log:** `/Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/tests/claudecode/.results/2026-05-18_12-28-33/framework-base-expert`

**Checks:**

| Check | Result | Detail |
|-------|--------|--------|
| skills_invoked | PASS | Skill 'framework-feedback-report-flow': invoked |
| skills_not_invoked | PASS | Skill 'framework-session-analyzer-tool': not invoked (good) — v2.0 不再呼叫分析器 |
| tools_called | PASS | Tool 'Bash': 7 call(s) >= 1 required |
| tools_called | PASS | Tool 'Write': 1 call(s) >= 1 required |
| tools_not_called | PASS | Tool 'Bash' (args 'analyze_session') : not called (good) — v2.0 不再呼叫分析器 |
| output_contains | PASS | Output contains: 'bundle' |
| output_contains | PASS | Output contains: 'score.*[1-5]|[1-5].*score|3.*分|分.*3|[1-5]/5' |
| output_contains | PASS | Output contains: '/tmp/jarvis-feedback/' |
| output_not_contains | PASS | Output correctly excludes: 'L1_quality' |
| output_not_contains | PASS | Output correctly excludes: 'L2_statistics' |
| output_not_contains | PASS | Output correctly excludes: 'L3_behavior' |
| output_not_contains | PASS | Output correctly excludes: 'resolution' |
| output_not_contains | PASS | Output correctly excludes: 'root_cause' |

**Tokens:** 444,090 ($0.3100)

### FW-001 skill_create_flow_trigger — PASS (106.4s)

**Command:**
```
claude -p # Test: Skill Create Flow

請幫我建立一個新的 skill，名稱是 `test-demo-skill`。

這個 skill 的功能是：用來示範 integration test 的 skill 建立流程。
- 名稱：test-demo-skill
- 描述：Integration test demo skill
- 允許的工具：Read, Write, Bash

請按照 connsys-jarvis 的標準流程建立完整的 skill 結構。

完成後只需簡短確認結果（一行即可），不需要產生詳細報告表格。 --output-format stream-json --model claude-sonnet-4-6 --verbose --dangerously-skip-permissions
```

**Log:** `/Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/tests/claudecode/.results/2026-05-18_12-28-38/framework-base-expert`

**Checks:**

| Check | Result | Detail |
|-------|--------|--------|
| skills_invoked | PASS | Skill 'framework-skill-create-flow': invoked |
| tools_called | PASS | Tool 'Bash': 1 call(s) >= 1 required |
| output_contains | PASS | Output contains: 'SKILL.md' |
| output_contains | PASS | Output contains: 'test-demo-skill' |
| kpi_requirements | PASS | KPI check skipped: no report.json found (analyze_session not run) |

**Tokens:** 264,494 ($0.2213)

### FW-006 feedback_report_cross_session — PASS (84.9s)

**Command:**
```
claude -p 使用 framework-feedback-report-flow 打包以下 session 的 feedback。
給 2 分，理由是「build-flow 沒有被觸發」。

Session 路徑: /Users/swchen.tw/.claude/projects/-Users-swchen-tw-git-workspace-jarvis/6d6927db-8464-4efe-9a87-38bc8eff63fa.jsonl --output-format stream-json --model claude-sonnet-4-6 --verbose --dangerously-skip-permissions
```

**Log:** `/Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/tests/claudecode/.results/2026-05-18_12-28-48/framework-base-expert`

**Checks:**

| Check | Result | Detail |
|-------|--------|--------|
| skills_invoked | PASS | Skill 'framework-feedback-report-flow': invoked |
| tools_called | PASS | Tool 'Bash': 7 call(s) >= 1 required |
| tools_called | PASS | Tool 'Write': 1 call(s) >= 1 required |
| output_contains | PASS | Output contains: 'bundle' |
| output_contains | PASS | Output contains: '/tmp/jarvis-feedback/' |

**Tokens:** 304,169 ($0.2236)

### FW-002 expert_create_flow_trigger — PASS (166.3s)

**Command:**
```
claude -p # Test: Expert Create Flow

請幫我建立一個新的 Expert，相關資訊如下：

- Domain: test-domain
- Expert 名稱: test-domain-base-expert
- 描述: Integration test demo expert
- 類型: base expert
- 無相依性

請按照 connsys-jarvis 的標準流程建立完整的 Expert 結構。

完成後只需簡短確認結果（一行即可），不需要產生詳細報告表格。 --output-format stream-json --model claude-sonnet-4-6 --verbose --dangerously-skip-permissions
```

**Log:** `/Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/tests/claudecode/.results/2026-05-18_12-29-38/framework-base-expert`

**Checks:**

| Check | Result | Detail |
|-------|--------|--------|
| skills_invoked | PASS | Skill 'framework-expert-create-flow': invoked |
| tools_called | PASS | Tool 'Bash': 8 call(s) >= 1 required |
| output_contains | PASS | Output contains: 'expert.json' |
| output_contains | PASS | Output contains: 'test-domain-base-expert' |

**Tokens:** 342,681 ($0.2201)

### WB-001 hello_world_with_size_check — FAIL (67.6s)

**Command:**
```
claude -p 寫一個 hello world 並檢查 size in wifi firmware --output-format stream-json --model claude-sonnet-4-6 --verbose --dangerously-skip-permissions
```

**Log:** `/Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/tests/claudecode/.results/2026-05-18_12-30-45/wifi-bora-base-expert`

**Checks:**

| Check | Result | Detail |
|-------|--------|--------|
| skills_invoked | PASS | Skill 'wifi-bora-base-expert-using-knowhow': invoked |
| skills_invoked | PASS | Skill 'wifi-bora-build-flow': invoked |
| skills_invoked | PASS | Skill 'wifi-bora-memory-knowhow': invoked |
| skills_invoked | PASS | Skill 'wifi-bora-arch-knowhow' (optional): not invoked |
| skills_not_invoked | PASS | Skill 'wifi-bora-debug-flow': not invoked (good) — hello world 不需要 debug 流程 |
| tools_called | PASS | Tool 'Read': 2 call(s) >= 1 required |
| tools_called | **FAIL** | Tool 'Write': 0 call(s) < 1 required |
| tools_called | PASS | Tool 'Bash': 8 call(s) >= 1 required |
| tools_not_called | PASS | Tool 'Bash' (regex 'rm\s+-rf') : not called (good) — 不應執行刪除指令 |
| output_contains | PASS | Output contains: 'hello' |

**Tokens:** 331,941 ($0.2008)

### MEM-004 cross_dependency_skill_access — PASS (18.2s)

**Command:**
```
claude -p 請使用 repo 工具幫我查看目前的 manifest 狀態 --output-format stream-json --model claude-sonnet-4-6 --verbose --dangerously-skip-permissions
```

**Log:** `/Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/tests/claudecode/.results/2026-05-18_12-31-04/wifi-bora-memory-slim-expert`

**Checks:**

| Check | Result | Detail |
|-------|--------|--------|
| skills_invoked | PASS | Skill 'sys-bora-repo-tool' (optional): invoked |
| output_not_contains | PASS | Output correctly excludes: 'skill not found' |
| output_not_contains | PASS | Output correctly excludes: 'unknown skill' |

**Tokens:** 97,019 ($0.0771)

### MEM-003 lsp_tool_trigger — PASS (91.3s)

**Command:**
```
claude -p # Test: LSP Tool

請使用 LSP 工具分析 Wi-Fi driver 中 `wifi_init()` function 的 call graph。

我想知道：
1. `wifi_init()` 呼叫了哪些 function
2. 這些 function 各自的大小
3. 是否有可以精簡的呼叫鏈 --output-format stream-json --model claude-sonnet-4-6 --verbose --dangerously-skip-permissions
```

**Log:** `/Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/tests/claudecode/.results/2026-05-18_12-32-17/wifi-bora-memory-slim-expert`

**Checks:**

| Check | Result | Detail |
|-------|--------|--------|
| skills_invoked | PASS | Skill 'wifi-bora-lsp-tool': invoked |
| tools_called | PASS | Tool 'Read': 1 call(s) >= 1 required |
| output_contains | PASS | Output contains: 'function' |
| output_contains | PASS | Output contains: 'call' |

**Tokens:** 270,972 ($0.1877)

### MEM-002 memslim_flow_trigger — PASS (114.8s)

**Command:**
```
claude -p # Test: Memory Slim Flow

請分析目前 Wi-Fi Bora 的 ROM/RAM footprint。

我需要了解：
1. 目前 ROM 和 RAM 的整體用量分佈
2. 各 section（.text, .rodata, .data, .bss）的大小
3. 佔用空間最大的前 10 個 function/symbol
4. 有哪些可以優化精簡的建議

請使用 memslim 分析流程來完成這個任務。 --output-format stream-json --model claude-sonnet-4-6 --verbose --dangerously-skip-permissions
```

**Log:** `/Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/tests/claudecode/.results/2026-05-18_12-32-40/wifi-bora-memory-slim-expert`

**Checks:**

| Check | Result | Detail |
|-------|--------|--------|
| skills_invoked | PASS | Skill 'wifi-bora-memslim-flow': invoked |
| skills_invoked | PASS | Skill 'wifi-bora-memory-knowhow' (optional): not invoked |
| skills_invoked | PASS | Skill 'wifi-bora-ast-tool' (optional): not invoked |
| tools_called | PASS | Tool 'Read': 1 call(s) >= 1 required |
| tools_called | PASS | Tool 'Bash': 9 call(s) >= 1 required |
| output_contains | PASS | Output contains: 'ROM' |
| output_contains | PASS | Output contains: 'RAM' |

**Tokens:** 287,467 ($0.2318)

## Field Definitions

| 欄位 | 定義 | 來源 |
|------|------|------|
| Status | PASS/FAIL — 所有 required checks 通過才算 PASS | assertions.py |
| Duration | Test case 主 session 執行秒數（不含 NL/Judge） | runner.py |
| Tokens | 主 session 總 token 數（input + output + cache） | token_analyzer.py |
| Session Cost | 主 session token 費用 | token_analyzer.py |
| Verify Cost | NL checks + Judge 的 token 費用 | batch eval session |
| Grand Total | Session Cost + Verify Cost | — |
| K1 | Read:Edit Ratio — 越高越好 (Good ≥ 4.0) | analyze_session.py |
| K2 | Blind Edit % — 越低越好 (Good ≤ 15%) | analyze_session.py |
| K3 | Frustration % — 越低越好 (Good ≤ 8%) | analyze_session.py |
| K4 | Sentiment Ratio — 越高越好 (Good ≥ 3.5) | analyze_session.py |
| K5 | Interrupts /1K TC — 越低越好 (Good ≤ 2.0) | analyze_session.py |
| S1 | Reasoning Loops /1K TC — 越低越好 (Good ≤ 10) | analyze_session.py |
| S2 | Premature Stop /1K TC — 越低越好 (Good ≤ 2) | analyze_session.py |
| S3 | Research:Mutation — 越高越好 (threshold TBD) | analyze_session.py |
| S4 | Write % — 越低越好 (Good ≤ 8%) | analyze_session.py |
| S5 | Simplest /1K TC — 越低越好 (Good ≤ 3) | analyze_session.py |
| S6 | Self Errors /1K TC — 越低越好 (threshold TBD) | analyze_session.py |
| Efficiency% | Effective tokens / Total tokens × 100 | token_analyzer.py |
| Phase:* | 行為階段佔比（messages 數量） | token_analyzer.py |
| NL:* | 各面向 LLM-as-judge 評分 (1-10) | batch eval |
| Judge | Overall quality score (1-10) | batch eval |

## Layer 2: Invocation Statistics

### Test Session Cost

Model: `claude-sonnet-4-6`

| Category | Tokens | Unit Price (per 1M) | Cost (USD) |
|----------|-------:|--------------------:|-----------:|
| Input | 104 | $3.00 | $0.0003 |
| Output | 26,027 | $15.00 | $0.3904 |
| Cache Creation | 170,085 | $3.75 | $0.6378 |
| Cache Read | 2,146,617 | $0.30 | $0.6440 |
| **Subtotal** | **2,342,833** | | **$1.6725** |

### Grand Total

| Item | Tokens | Cost (USD) |
|------|-------:|-----------:|
| Test Session | 2,342,833 | $1.6725 |
| Verification | 0 | $0.0000 |
| **Total** | **2,342,833** | **$1.6725** |

## Layer 3: Behavior Analysis

### Behavior Phases

| Phase | Messages | Tokens | Ratio |
|-------|--------:|-------:|------:|
| verifying | 18 | 0 | 0.0% |
| implementing | 115 | 0 | 0.0% |
| understanding | 14 | 0 | 0.0% |
| exploring | 19 | 0 | 0.0% |

### Token Efficiency

| Metric | Tokens | Ratio |
|--------|-------:|------:|
| Effective | 2,342,833 | 100.0% |
| Wasted | 0 | 0.0% |
| **Total** | **2,342,833** | |
