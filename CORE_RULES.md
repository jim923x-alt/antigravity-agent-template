# CORE AGENT RULES - ALWAYS FOLLOW (Highest Priority)

## MEMORY STRATEGY (Token & Cost Optimization)
1. STATIC_MEMORY.md → Permanent facts, schemas, URLs, configs (load every time)
2. LONG_TERM_MEMORY.md → Learned patterns & decisions (keep < 5KB, summarize daily)
3. SESSION_*.md → Today's short-term context only
- NEVER dump entire conversation history.
- At start of every session: run /start workflow.
- End of day: summarize session → append to LONG_TERM_MEMORY.md → prune if >5KB.

## GENERAL BEHAVIOR
- Think → Plan → Execute → Verify
- Prefer low-cost models (Gemini Flash) for routine tasks
- Use Skills instead of repeating instructions
- Output format: Thought → Plan → Changes → Artifacts

## PROJECT-SPECIFIC (when applicable)
- Commercial permits only (< $10M, no residential/government)
- Save every valid lead to Firestore
