# 1️⃣ Deterministic writing

This reference document serves as the absolute standard for transforming implicit, ambiguous human communication into clear, deterministic logic.  
Use these matrices to refine documentation, code review comments, and engineering prompts for Claude Code.  

---

## 👁️‍🗨️ The clear English version (Ambiguous vs. Unambiguous)

| Step name | Ambiguous writing | Unambiguous writing | Why it is better? |
| :--- | :--- | :--- | :--- |
| Refine Your Structure | Cut the wood with the saw and clean it. | Cut the wood with the saw, then clean the saw. | Clarifies what "it" refers to. Repeating the noun removes ambiguity. |
| Choose Precise Words (Time) | Call me when you are free. | Call me on Wednesday at 2:00 PM. | Removes timeline guesswork. Vague schedules cause missed connections. |
| Choose Precise Words (Pronouns) | The patient told the doctor she was sick. | The patient said that the doctor was sick. | Identifies the correct person. Confusing pronouns mask the subject. |
| Master Punctuation (Hyphens) | He saw a man eating shark. | He saw a man-eating shark. | Clarifies the descriptive words. Hyphens connect a single concept. |
| Master Punctuation (Lists) | I love my parents, Taylor Swift and Barack Obama. | I love my parents, Taylor Swift, and Barack Obama. | Separates list items clearly. The Oxford comma prevents accidental grouping. |
| Enforce Active Voice | The system code was rewritten to fix bugs. | The senior developer rewrote the system code to fix bugs. | Explicitly names the actor. Passive voice hides who did what. |
| Quantify Goals & Limits | Make this code run faster and keep the explanation short. | Reduce execution time below 200ms and limit the explanation to 3 bullet points. | Replaces opinions with metrics. Relative words mean different things to AI. |
| Verify System Outputs | Check everything — test everything and from many angles. | Assume the code has failed by default. Test each function against explicit edge cases, missing parameters, and invalid data types to prove a pass. | Overturns the model's natural bias to be overly agreeable. Enforcing strict boundary states blocks unexpected runtime behavior. Demanding active proof of correctness catches hidden bugs. |

---

## 🤖 The highly precise programmatic version

| Objective / phase | Indeterminate input (implicit) | Deterministic input (explicit) | Structural optimisation and impact |
| :--- | :--- | :--- | :--- |
| Contextual Scoping | Cut the wood with the saw and clean it. | Cut the wood with the saw, then clean the saw. | Eliminates pronoun resolution failures. Noun repetition prevents execution state drift. |
| Temporal Parameterization | Call me when you are free. | Call me on Wednesday at 2:00 PM. | Mitigates timeline heuristics guessing. Unbounded parameters degrade scheduling reliability. |
| Subject-Object Resolution | The patient told the doctor she was sick. | The patient said that the doctor was sick. | Enforces deterministic entity linking. Amorphous pronoun mapping introduces systemic bias. |
| Syntactic Token Binding | He saw a man eating shark. | He saw a man-eating shark. | Adjusts semantic token grouping via grammar. Compound modifiers bind distinct tokens safely. |
| Array Boundary Isolation | I love my parents, Taylor Swift and Barack Obama. | I love my parents, Taylor Swift, and Barack Obama. | Demarcates collection boundaries explicitly. The serial delimiter blocks invalid structural nesting. |
| Actor-Action Attribution. (Active) | The system code was rewritten to fix bugs. | The senior developer rewrote the system code to fix bugs. | Enforces direct execution trace tracking. Passive syntax structures obscure the executing agent. |
| Metric Constraint Enforcement | Make this code run faster and keep the explanation short. | Reduce execution time below 200ms and limit the explanation to 3 bullet points. | Swaps qualitative tokens for static thresholds. Relative descriptors break model scoring heuristics. |
| Validation Architecture | Check everything — test everything and from many angles. | Initialize the test suite with a default fail-closed state. Enforce boundary-value testing across all component inputs, rejecting unverified executions. | Neutralizes sycophancy patterns by establishing a pessimistic baseline. Enforcing strict boundary states blocks unexpected runtime behavior. Treating ambiguous execution tokens as hard failures ensures pipeline integrity. |

---

## ▶️ Core execution phrase  
When flagging unvalidated, loose constraints or vague references in files or code reviews, insert the following baseline reminder:

> ### ❓ Who/What Did What
> To write unambiguously, you must explicitly state who or what did what. Clearly naming the exact subject and action eliminates guesswork and forces AI to deliver perfectly deterministic results.
  

Yes, the number 1 can symbolize deterministic writing by representing a single, unalterable path or a rigid binary foundation where only one outcome is possible.Why the Number 1 Works as a SymbolSingularity: The number 1 stands for a single truth or a singular, non-negotiable path. Determinism relies on the idea that history or a text has only one way to unfold.Binary Logic: In digital systems and formal logic, a sequence built on 1s and 0s represents a closed system. Every action and output is strictly fixed by a rule, leaving no room for random chance.Order Versus Chaos: Writers use the number 1 to show absolute control, fate, or a strict mechanical order that opposes chaotic or free-willed writing.  
