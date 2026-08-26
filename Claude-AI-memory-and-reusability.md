# ✨ Claude AI memory and reusability  


Claude AI memory is stored in CLAUDE.md Markdown file in the main project folder.  
You can use it to store information without reasking.  
  
More memory can be imported and you can have reusable flows called skills.  
  
### 🧠 Claude.md example
``` 
# Test project.

## Imported memory.
@domain-knowledge.md  
@report-format.md  
@data-sources.md  

## Core behavior
1. Answers must follow instructions from imported memories.
2. Run only what's asked.
3. Use /run-all-tests to do all testing.
```

### domain-knowledge.md additional memory example
```
# Domain Knowledge

1. "Analysis accuracy" is analysis output versus actual evidence found.
2. "Test coverage" are all test types from the test strategy (structural, functional, etc).
3. Known past issues are evidence and scenario count mismatches.
```

### .claude/skills/run-all-tests/SKILL.md reusable flow
```
---
description: Run all tests in order.
---
# Run all tests.
1. Run get-analysis-accuracy skill.
2. Run get-test-coverage skill.
3. Run report-test-strategy-suggestions skill using outputs from 1 and 2.
4. Create a combined report using report-format.md.
```
