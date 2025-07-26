# Vue.js Training Project Tasks

## Active Tasks (Current Sprint)

*No active tasks currently*

---

## Backlog (Future Work)

### Learning Examples & Features
- [ ] **P2** T001 [S] [Claude] Add Vue 3 Composition API examples
  - Create standalone examples using setup() function
  - Demonstrate reactive variables and computed properties
- [ ] **P2** T002 [S] [Unassigned] Create component communication examples  
  - Parent-child component examples with props and events
  - Demonstrate component composition patterns
- [ ] **P3** T003 [M] [Unassigned] Add advanced Vue features examples
  - Custom directives, filters, and mixins
  - Vue Router integration for single-page navigation
- [ ] **P3** T004 [S] [Unassigned] Create form handling and validation examples
  - Complex forms with validation using v-model
  - File upload and form submission examples

### Code Organization & Quality  
- [ ] **P2** T005 [S] [Unassigned] Improve code consistency across examples
  - Standardize JavaScript formatting and naming conventions
  - Ensure consistent Bootstrap integration patterns
- [ ] **P3** T006 [S] [Unassigned] Add responsive design improvements
  - Test and improve mobile compatibility
  - Add more advanced Bootstrap responsive examples

### Vue Version Updates
- [x] ✅ **P1** T009 [S] [Claude] Prepare Vue update environment (2025-07-25)
  - ✅ Check latest Vue 3 version and migration guide (Vue 3.5.18)
  - ✅ Create git branch: `vue-update`
  - ✅ Review breaking changes documentation
- [x] ✅ **P1** T010 [S] [Claude] Download and integrate new Vue version (2025-07-25)
  - ✅ Download latest `vue.esm-browser.js` from Vue CDN
  - ✅ Rename to version-specific filename: `vue.esm-browser-3-5-18.js`
  - ✅ Update import statements in all 9 vue_*.html files
- [x] ✅ **P1** T011 [M] [Claude] Test basic Vue examples after update (2025-07-25)
  - ✅ Test vue_1_einbinden.html and vue_2_evaluate_expression.html
  - ✅ Test vue_3_input_field_and_databinding.html
  - ✅ No breaking changes or console errors found
- [x] ✅ **P1** T012 [M] [Claude] Test advanced Vue features after update (2025-07-25)
  - ✅ Test lifecycle hooks (vue_6_use_mounted_hook.html)
  - ✅ Test v-for iterations (vue_7_iterate_with_v-for.html)
  - ✅ Test Bootstrap integration examples
- [ ] **P2** T013 [S] [Claude] Update documentation for new Vue version [Details](./session-state-vue-update.md)
  - Update README.md with new Vue version
  - Update CLAUDE.md project description
  - Update HTML file header comments
- [ ] **P2** T014 [S] [Unassigned] Final validation and cleanup
  - Test all examples in multiple browsers
  - Verify responsive behavior
  - Commit changes and merge to main

### Project Quality
- [x] ✅ **P2** T015 [S] [Claude] Create concise style guide for Vue project (2025-07-25)
  - ✅ Vue.js Official Style Guide standards
  - ✅ JavaScript Standard Style formatting
  - ✅ Learning-focused guidelines with TOC

### Learning Resources
- [ ] **P2** T007 [M] [Unassigned] Create comprehensive learning guide
  - Document recommended order for studying examples  
  - Add detailed concept explanations for each file
- [ ] **P3** T008 [S] [Unassigned] Add practice exercises
  - Create coding challenges based on each example
  - Include solution files with explanations

---

## Completed Tasks (Archive)

- [x] ✅ **P1** T021 [S] [Claude] Add visual explanation to vue_2_evaluate_expression.html (2025-07-26)
  - ✅ Added interactive input fields with v-model for real-time expression updates
  - ✅ Created comprehensive explanation card showing how Vue expression evaluation works
  - ✅ Added concrete examples: `{{ x }}` → variable, `{{ x * y }}` → calculation, `{{ "Hello!" }}` → literal text
  - ✅ Enhanced learning progression from vue_1 (integration) to vue_2 (expressions + interactivity)

---

## Task Management Guidelines

### Task Format
```
- [ ] **P[1-4]** T[###] [S/M/L/XL] [AI] Description [Depends on T###] [Link to details]
```

**Components:**
- **Priority**: P1 (Critical) → P4 (Low)
- **Task ID**: T001, T002, T003... (sequential, project-specific)
- **Size**: S(mall), M(edium), L(arge), XL (epic)
- **AI**: Claude, Cursor, VS, Other (which assistant is assigned/working)
- **Dependencies**: [Depends on T###] (optional)
- **Details**: [Planning Document](./planning/task-details-T###.md) (optional)

### Task Lifecycle
1. **Backlog** → **Active** (when work begins)
2. **Active** → **Completed** (when finished)
3. **Completed** tasks move to archive (most recent first)

### Linking Strategy
- **Keep TASKS.md lightweight**: Brief descriptions only
- **Detailed planning**: Create separate files in `tasks/planning/` folder
- **Reference format**: `[Details](./planning/T001-feature-implementation.md)`
- **Epic breakdown**: Link to planning documents for complex features

### Multi-AI Collaboration
- **AI Assignment**: Mark which assistant is working on each task
- **Handoff Protocol**: Update status when passing tasks between AIs
- **Session Tracking**: Reference session logs in task comments when needed
- **Context Sharing**: Use this unified file for all assistants to see full picture

### Examples
```markdown
## Active Tasks
- [ ] **P1** T003 [M] [Claude] Implement user authentication system [Details](./planning/T003-auth-system.md)
- [ ] **P2** T005 [S] [Cursor] Fix responsive layout issues

## Backlog  
- [ ] **P1** T001 [L] Setup database connection and migrations [Depends on T003]
- [ ] **P3** T004 [S] Add unit tests for user service

## Completed Tasks
- [x] ✅ **P1** T002 [S] [Claude] Setup project documentation structure (2025-01-22)
```
