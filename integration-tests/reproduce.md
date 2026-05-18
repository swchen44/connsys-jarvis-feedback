# Reproduce Guide

## Original Command
```bash
python3 -m tests.claudecode --all --session-analysis ai --upload
```

---

## Per-Case Commands

### framework-base-expert / FW-002: expert_create_flow_trigger

#### Prerequisites
```bash
python3 /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/scripts/setup.py --add /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/framework/framework-base-expert/expert.json
```

#### Quick Run (no eval)
```bash
python3 -m tests.claudecode --expert framework-base-expert -t FW-002 --skip-eval --session-analysis none
```

#### Original Headless Command
```bash
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

### Environment
- Model: claude-sonnet-4-6
- Mode: headless
- Timeout: 300s
- Working Directory: /Users/swchen.tw/git/workspace_jarvis

---

### framework-base-expert / FW-001: skill_create_flow_trigger

#### Prerequisites
```bash
python3 /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/scripts/setup.py --add /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/framework/framework-base-expert/expert.json
```

#### Quick Run (no eval)
```bash
python3 -m tests.claudecode --expert framework-base-expert -t FW-001 --skip-eval --session-analysis none
```

#### Original Headless Command
```bash
claude -p # Test: Skill Create Flow

請幫我建立一個新的 skill，名稱是 `test-demo-skill`。

這個 skill 的功能是：用來示範 integration test 的 skill 建立流程。
- 名稱：test-demo-skill
- 描述：Integration test demo skill
- 允許的工具：Read, Write, Bash

請按照 connsys-jarvis 的標準流程建立完整的 skill 結構。

完成後只需簡短確認結果（一行即可），不需要產生詳細報告表格。 --output-format stream-json --model claude-sonnet-4-6 --verbose --dangerously-skip-permissions
```

### Environment
- Model: claude-sonnet-4-6
- Mode: headless
- Timeout: 300s
- Working Directory: /Users/swchen.tw/git/workspace_jarvis

---

### framework-base-expert / FW-005: feedback_report_flow_trigger

#### Prerequisites
```bash
python3 /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/scripts/setup.py --add /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/framework/framework-base-expert/expert.json
```

#### Quick Run (no eval)
```bash
python3 -m tests.claudecode --expert framework-base-expert -t FW-005 --skip-eval --session-analysis none
```

#### Original Headless Command
```bash
claude -p 我有這個 skills framework-skill-create-flow 嗎？這個 skill 中提到要創建新的 skills 命名規則是什麼？

回答完後，請使用 framework-feedback-report-flow 幫我打包最新的 session 的 feedback。給 3 分，理由是「測試用途，驗證打包流程」。 --output-format stream-json --model claude-sonnet-4-6 --verbose --dangerously-skip-permissions
```

### Environment
- Model: claude-sonnet-4-6
- Mode: headless
- Timeout: 300s
- Working Directory: /Users/swchen.tw/git/workspace_jarvis

---

### framework-base-expert / FW-006: feedback_report_cross_session

#### Prerequisites
```bash
python3 /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/scripts/setup.py --add /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/framework/framework-base-expert/expert.json
```

#### Quick Run (no eval)
```bash
python3 -m tests.claudecode --expert framework-base-expert -t FW-006 --skip-eval --session-analysis none
```

#### Original Headless Command
```bash
claude -p 使用 framework-feedback-report-flow 打包以下 session 的 feedback。
給 2 分，理由是「build-flow 沒有被觸發」。

Session 路徑: /Users/swchen.tw/.claude/projects/-Users-swchen-tw-git-workspace-jarvis/526aa313-f5e5-4ad5-803b-469b7c1923d8.jsonl --output-format stream-json --model claude-sonnet-4-6 --verbose --dangerously-skip-permissions
```

### Environment
- Model: claude-sonnet-4-6
- Mode: headless
- Timeout: 300s
- Working Directory: /Users/swchen.tw/git/workspace_jarvis

---

### wifi-bora-base-expert / WB-001: hello_world_with_size_check

#### Prerequisites
```bash
python3 /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/scripts/setup.py --add /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/framework/wifi-bora-base-expert/expert.json
```

#### Quick Run (no eval)
```bash
python3 -m tests.claudecode --expert wifi-bora-base-expert -t WB-001 --skip-eval --session-analysis none
```

#### Original Headless Command
```bash
claude -p 寫一個 hello world 並檢查 size in wifi firmware --output-format stream-json --model claude-sonnet-4-6 --verbose --dangerously-skip-permissions
```

### Environment
- Model: claude-sonnet-4-6
- Mode: headless
- Timeout: 300s
- Working Directory: /Users/swchen.tw/git/workspace_jarvis

---

### wifi-bora-memory-slim-expert / MEM-002: memslim_flow_trigger

#### Prerequisites
```bash
python3 /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/scripts/setup.py --add /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/framework/wifi-bora-memory-slim-expert/expert.json
```

#### Quick Run (no eval)
```bash
python3 -m tests.claudecode --expert wifi-bora-memory-slim-expert -t MEM-002 --skip-eval --session-analysis none
```

#### Original Headless Command
```bash
claude -p # Test: Memory Slim Flow

請分析目前 Wi-Fi Bora 的 ROM/RAM footprint。

我需要了解：
1. 目前 ROM 和 RAM 的整體用量分佈
2. 各 section（.text, .rodata, .data, .bss）的大小
3. 佔用空間最大的前 10 個 function/symbol
4. 有哪些可以優化精簡的建議

請使用 memslim 分析流程來完成這個任務。 --output-format stream-json --model claude-sonnet-4-6 --verbose --dangerously-skip-permissions
```

### Environment
- Model: claude-sonnet-4-6
- Mode: headless
- Timeout: 300s
- Working Directory: /Users/swchen.tw/git/workspace_jarvis

---

### wifi-bora-memory-slim-expert / MEM-004: cross_dependency_skill_access

#### Prerequisites
```bash
python3 /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/scripts/setup.py --add /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/framework/wifi-bora-memory-slim-expert/expert.json
```

#### Quick Run (no eval)
```bash
python3 -m tests.claudecode --expert wifi-bora-memory-slim-expert -t MEM-004 --skip-eval --session-analysis none
```

#### Original Headless Command
```bash
claude -p 請使用 repo 工具幫我查看目前的 manifest 狀態 --output-format stream-json --model claude-sonnet-4-6 --verbose --dangerously-skip-permissions
```

### Environment
- Model: claude-sonnet-4-6
- Mode: headless
- Timeout: 300s
- Working Directory: /Users/swchen.tw/git/workspace_jarvis

---

### wifi-bora-memory-slim-expert / MEM-003: lsp_tool_trigger

#### Prerequisites
```bash
python3 /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/scripts/setup.py --add /Users/swchen.tw/git/workspace_jarvis/connsys-jarvis/framework/wifi-bora-memory-slim-expert/expert.json
```

#### Quick Run (no eval)
```bash
python3 -m tests.claudecode --expert wifi-bora-memory-slim-expert -t MEM-003 --skip-eval --session-analysis none
```

#### Original Headless Command
```bash
claude -p # Test: LSP Tool

請使用 LSP 工具分析 Wi-Fi driver 中 `wifi_init()` function 的 call graph。

我想知道：
1. `wifi_init()` 呼叫了哪些 function
2. 這些 function 各自的大小
3. 是否有可以精簡的呼叫鏈 --output-format stream-json --model claude-sonnet-4-6 --verbose --dangerously-skip-permissions
```

### Environment
- Model: claude-sonnet-4-6
- Mode: headless
- Timeout: 300s
- Working Directory: /Users/swchen.tw/git/workspace_jarvis

---
