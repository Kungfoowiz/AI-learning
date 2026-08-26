# ✨ Claude AI memory and reusability  


CLAUDE.md Markdown is Claude AI's memory.
You can use it to store information without reasking.
It lives in the main folder of your project.

You can separate guidance files, such as additional memory and reusable flows (skills).

### 🧠 Claude.md example
``` 
# Test project

## Imports
@.claude/domain-knowledge.md  
@.claude/report-format.md  
@.claude/data-sources.md  

## Core behavior
1. Ground answers in the guidance files above.
2. Run only what's asked.
3. Use /run-all-tests for the full chain.
```

### @.claude/domain-knowledge.md
```
# Domain Knowledge

1. What "analysis accuracy" means for this project (developer's
  analysis output vs. actual evidence found)
2. What "test coverage" means here (unit/integration/e2e breakdown)
3. Known past issues (e.g. evidence count mismatches)
```

### .claude/skills/run-all-tests/SKILL.md
```
---
description: Run the full test in order
---
# Run all tests
1. Run get-analysis-accuracy
2. Run get-test-coverage
3. Run report-test-strategy-suggestions (using outputs from 1 and 2)
Present combined, using .claude/report-format.md
```
