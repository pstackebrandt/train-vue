# Vue.js Training Project Style Guide

## Table of Contents
- [Purpose](#purpose)
- [Vue.js Standards](#vuejs-standards)
- [JavaScript Standards](#javascript-standards)
- [HTML Standards](#html-standards)
- [Bootstrap Integration](#bootstrap-integration)
- [Comments](#comments)
- [File Organization](#file-organization)

## Purpose
Minimal style conventions to maintain code consistency without disrupting learning objectives.

## Vue.js Standards
Follow [Vue.js Official Style Guide](https://vuejs.org/style-guide/) rules:

### Component Structure
```javascript
createApp({
  data() {
    return {
      // reactive data
    }
  },
  methods: {
    // event handlers
  },
  mounted() {
    // lifecycle hooks
  }
}).mount('#app');
```

### Template Directives
- Use `:` shorthand for `v-bind`
- Use `@` shorthand for `v-on`
- Always include `key` attribute in `v-for`

## JavaScript Standards
Based on [JavaScript Standard Style](https://standardjs.com/):

### Formatting
- 2 spaces for indentation
- Semicolons required
- Single quotes for strings
- No trailing commas in objects/arrays

### Naming
- `camelCase` for variables and functions
- `PascalCase` for component names (future)

## HTML Standards
- Use semantic HTML5 elements
- Include `alt` attributes for images
- Maintain proper heading hierarchy

## Bootstrap Integration
- Use standard Bootstrap 5 classes
- Maintain responsive design patterns
- Consistent spacing with utility classes

## Comments
- English for new code and explanations
- Keep existing German comments for learning continuity
- Document complex Vue patterns for educational purposes

## File Organization
- Maintain `vue_[number]_[description].html` naming
- Keep examples self-contained
- Include attribution comments as established