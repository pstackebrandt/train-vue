# AI Handoff Guide

## Purpose

Guidelines for seamless task handoffs between different AI assistants (Claude Code, Cursor AI, VS Code assistants) working on the Vue.js training project.

## Quick Reference

### Before Handoff (Current AI)
1. Update task status in TASKS.md
2. Document current state/progress
3. Log session summary
4. Commit/save all work in progress

### After Handoff (New AI)
1. Read TASKS.md for context
2. Review session logs
3. Check git status and recent commits
4. Update task assignment

## Detailed Handoff Process

### 1. Preparation (Outgoing AI)

**Update Task Status:**
```markdown
# Change from:
- [ ] **P2** T002 [S] [Claude] Create component communication examples

# To:
- [ ] **P2** T002 [S] [Claude→Cursor] Create component communication examples [Basic props example completed, need events example]
```

**Document Progress:**
- What's been completed
- Current blockers or decisions needed
- Files modified
- Next logical steps

**Session Log Entry:**
```markdown
## Claude Session - 2025-01-25

### T002: Component Communication Examples
- ✅ Created parent-child props example
- ✅ Added data passing demonstration
- 🔄 Started event handling example (50% complete)
- ❌ Component composition patterns not started
- **Next**: Complete event example, add composition patterns
- **Files**: vue_8_parent_child_props.html, vue_9_event_handling.html
- **Branch**: T002-component-communication
```

### 2. Context Transfer (Incoming AI)

**Read Current State:**
```bash
# 1. Check active tasks
grep -A 5 "Active Tasks" tasks/TASKS.md

# 2. Review recent session logs
tail -20 tasks/session-logs/claude-sessions.md

# 3. Check git status
git status
git log --oneline -10
```

**Update Assignment:**
```markdown
# Change from:
- [ ] **P2** T002 [S] [Claude→Cursor] Create component communication examples [Basic props example completed, need events example]

# To:  
- [ ] **P2** T002 [S] [Cursor] Create component communication examples [Continuing from Claude: props done, working on events]
```

## Session Logging Templates

### Starting Session Template
```markdown
## [AI] Session - [Date]

### Session Goals
- [ ] Complete T### task
- [ ] Fix issue X
- [ ] Start work on Y

### Handoff Context (if applicable)
- Previous AI: [Name]
- Current state: [Description]
- Files to focus on: [List]
```

### Ending Session Template  
```markdown
### Session Summary
- ✅ Completed: [List achievements]  
- 🔄 In Progress: [Current work state]
- ❌ Blocked: [Issues encountered]
- **Next Session**: [Recommended next steps]
- **Files Modified**: [List]
- **Commits**: [Commit hashes if applicable]

### Notes for Next AI
- [Context, decisions, gotchas]
```

## Common Handoff Scenarios

### 1. Mid-Task Handoff
**Situation**: Complex task needs to continue with different AI

**Process**:
- Document exactly where you stopped
- List files in progress (uncommitted changes)
- Describe approach taken so far
- Suggest next steps

**Example**:
```markdown
T003 [M] [Claude→Cursor] Advanced Vue features examples [Basic directives created, need router integration]
- ✅ Created custom directive examples  
- ✅ Added filter demonstration
- 🔄 Working on Vue Router integration (vue_10_router.html 30% done)
- **Next**: Complete router example, add navigation patterns
- **Uncommitted**: vue_10_router.html, vue_11_advanced_directives.html
```

### 2. Different Expertise Handoff
**Situation**: Task requires different AI's strengths

**Process**:
- Explain why handoff is beneficial
- Provide full context of technical decisions
- Hand over cleanly completed portions

**Example**:
```markdown  
T001 [S] [Claude→Cursor] Vue Composition API examples [Basic reactive setup done, need advanced patterns]
- ✅ Created basic setup() function examples
- ✅ Added reactive variables demonstration  
- ✅ Included computed properties examples
- **Handoff Reason**: Need advanced Vue 3 patterns expertise
- **Next**: Add advanced composable patterns, lifecycle hooks integration
```

### 3. Blocked Task Handoff
**Situation**: Current AI is blocked, another might have solution

**Process**:
- Document the blocker clearly
- Explain attempts made to resolve
- Suggest alternative approaches

## File Management During Handoffs

### Work in Progress Files
- **Commit partial work** with clear commit messages
- **Use feature branches** named after task IDs
- **Document uncommitted changes** in handoff notes

### Session State Preservation
```bash
# Before ending session
git add .
git commit -m "T002: WIP - Props example completed, event handling started"
git push origin T002-component-communication

# Note in handoff:
# "Branch T002-component-communication has latest work, vue_9_event_handling.html needs completion"
```

## Best Practices

### For Smooth Handoffs

1. **Be Explicit**: Don't assume next AI understands context
2. **Document Decisions**: Why you chose approach X over Y  
3. **List Dependencies**: What other tasks/files this affects
4. **Provide Examples**: Show format/patterns you've established
5. **Update Immediately**: Don't delay updating TASKS.md

### Communication Style
- Use clear, factual language
- Avoid subjective opinions ("I think", "maybe")
- Focus on actionable information
- Include file paths and line numbers when relevant

### Common Mistakes to Avoid
- ❌ Leaving tasks in "Active" without progress notes
- ❌ Not documenting current approach/reasoning  
- ❌ Forgetting to update AI assignment in TASKS.md
- ❌ Leaving uncommitted changes without explanation
- ❌ Not providing enough context for continuation

## Emergency Handoffs

### Session Crash/Unexpected Termination

**If Previous AI Session Crashed:**
1. Check git log for last commits
2. Look for any session logs from that day
3. Check file modification times  
4. Read TASKS.md for last known status
5. Start conservatively - understand before changing

**Recovery Steps:**
```bash
# Check what was being worked on
git log --since="1 day ago" --oneline
git status
find . -name "*.html" -mtime -1  # Files modified in last day

# Review task file
grep -n "T0" tasks/TASKS.md | grep -v "✅"  # Find active tasks
```

## Integration with Claude Code

### Resuming After Claude Code Crashes
- Use `claude-code --resume` to restore session context
- Check if task status in TASKS.md matches actual progress  
- Verify git state matches documented progress
- Update session logs with any recovery actions needed