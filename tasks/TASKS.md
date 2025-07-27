# Vue.js Training Project Tasks

## Active Tasks (Current Sprint)

- [x] ✅ **P2** T022 [M] [Claude] Review and update remaining vue_n files for consistency and educational value (2025-07-27)
  - [x] ✅ **P1** T027 [S] [Claude] Fix vue_4_use_conditional_evaluation.html - remove German boilerplate comments (2025-07-27)
  - [x] ✅ **P1** T028 [M] [Claude] Update vue_5_show_image_databinding_bootstrap.html - consistent styling, explanations, Bootstrap version (2025-07-27)
  - [x] ✅ **P1** T029 [M] [Claude] Update vue_5b_show_images_databinding_method.html - English method names, consistent structure (2025-07-27)
  - [x] ✅ **P1** T030 [M] [Claude] Update vue_6_use_mounted_hook.html - English method names, consistent structure (2025-07-27)
  - [x] ✅ **P1** T031 [L] [Claude] Completely rebuild vue_7_add_image.html - fix broken structure, rename to vue_7_dynamic_content_addition.html (2025-07-27)

- [x] ✅ **P2** T032 [M] [Claude] Add Vue API markers and format sections to all vue files [Details](./planning/T032-vue-api-markers.md) (2025-07-27)
  - [x] ✅ **P2** T032a [S] [Claude] Test API marker implementation on vue_6_use_mounted_hook.html (2025-07-27)
  - [x] ✅ **P2** T032c [S] [Claude] Create DEVELOPER_GUIDE.md with file structure standards (2025-07-27)
  - [x] ✅ **P2** T032d [S] [Claude] Update STYLE_GUIDE.md with API marker standards (2025-07-27)
  - [x] ✅ **P2** T032e [S] [Claude] Update T032 planning document for file-specific approach (2025-07-27)
  - [x] ✅ **P2** T032f [S] [Claude] Implement file-specific format sections for vue_1 and vue_6 (2025-07-27)
  - [x] ✅ **P2** T032g [M] [Claude] Update remaining 8 vue files with API markers and file-specific formats (2025-07-27)

- [x] ✅ **P2** T033 [S] [Claude] Update Purpose section language for accurate positioning (2025-07-27)
  - [x] ✅ **P2** T033a [S] [Claude] Update DEVELOPER_GUIDE.md with educational language guidelines (2025-07-27)
  - [x] ✅ **P2** T033b [S] [Claude] Update all Purpose sections with varied semantic language (2025-07-27)

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

- [x] ✅ **P1** T023 [M] [Claude] Improve vue_3_input_field_and_databinding.html for better 2-way binding demo (2025-07-26)
  - ✅ Updated comments: Removed outdated German boilerplate, added v-model specific explanations
  - ✅ Added methods with demonstration buttons: setExampleValues() and resetValues() for programmatic data changes
  - ✅ Enhanced interactivity: Shows both binding directions (Input → Data and Code → Input)
  - ✅ Added visual explanation: "How v-model Two-Way Binding Works" with concrete examples
  - ✅ Marked v-model usage locations with comments for clarity
  - ✅ Updated Content section: "v-model directive, bidirectional binding, methods, @click events, programmatic data updates"

- [x] ✅ **P2** T024 [M] [Claude] Clean up npm artifacts and enhance README with GitHub Pages deployment info (2025-07-27)
  - ✅ Removed package.json and package-lock.json (misleading npm artifacts)
  - ✅ Enhanced README.md with "What This Is / What This Is NOT" sections
  - ✅ Added author attribution and educational value section
  - ✅ Created DEPLOYMENT.md with comprehensive GitHub Pages hosting guide
  - ✅ Renamed Readme.md to README.md and removed job interview references

- [x] ✅ **P2** T033 [S] [Claude] Update Purpose section language for accurate positioning (2025-07-27)
  - ✅ Updated DEVELOPER_GUIDE.md with educational language guidelines
  - ✅ Documented rationale for avoiding "Learn how to..." phrasing
  - ✅ Provided approved phrases with linguistic variety
  - ✅ Updated all 10 vue files with varied Purpose section language
  - ✅ Positioned files as supplementary examples, not standalone lessons

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
