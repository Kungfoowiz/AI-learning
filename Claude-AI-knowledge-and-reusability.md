# ✨ Claude AI memory and reusability  


Claude AI's knowledge is stored in CLAUDE.md Markdown file in the main project folder.  
It stores learning without you reasking Claude AI.  
More learning can be added and you can also have reusable flows called skills.  
  
### 🧠 Claude.md example
``` 
# Test project.

## My learning.
@focus.md  
@report-format.md  
@data.md  

## How I work?
1. Answers must follow instructions from my learning.
2. Run only what's asked.
3. Use /run-all-tests to do all testing.
```

### focus.md example
```
# Focus

1. "Analysis accuracy" is actual analysis checked against evidence.
2. "Test coverage" is calculated in percentages of all types of testing from a test strategy.
3. Known past issues were incorrect evidence and scenario counts from actual analysis.
```

### report-format.md example
```
# Report format

Reports should:
1. State what was measured.
2. Show numbers plainly, examples: found vs. expected, coverage %.
3. Flag bugs clearly, do not hide anything.
4. Suggest next steps only when we need to do something.
```

### data.md example
```
# Data
1. Always ask the user to confirm all actual input to reusable flows.
2. Always ask the user to confirm all expected output to reusable flows.
3. Test coverage comes from checking the code.
4. Missing or bad data is flagged as a bug.
```

### .claude/skills/get-analysis-accuracy/SKILL.md reusable flow
```
---
description: Get analysis accuracy.
---
# Get analysis accuracy.
1. Use the rules in data.md.
1. Load the actual inputted analysis.
2. Count the number of actual evidences.
3. Compare it to the number of evidences the user found in expected output.
4. Show the analysis evidence count, the expected evidence count and bugs.
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
