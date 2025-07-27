# Vue.js Training Project Style Guide

## Table of Contents
- [Purpose](#purpose)
- [Vue.js Standards](#vuejs-standards)
- [API Markers](#api-markers)
- [Educational Structure](#educational-structure)
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

## API Markers

### Icon Standards
- **Options API**: ⚙️ (gear) - represents configuration/options approach
- **Future Composition API**: 🧩 (puzzle piece) - represents composable functions

### Content Card Integration
Add API marker to Content card title with link to format section:

```html
<h5 class="card-title text-secondary">
  🔧 Content | 
  <a href="#format-section" class="text-decoration-none text-info">
    ⚙️ Options API
  </a>
</h5>
```

### Format Section Structure
Each file must include a file-specific format section:

```html
<!-- Vue Options API Format Reference -->
<div class="mt-4">
  <div id="format-section" class="card border-info">
    <div class="card-header bg-info text-white">
      <h4 class="card-title mb-0">⚙️ Vue Options API Format</h4>
    </div>
    <div class="card-body">
      <pre class="bg-light p-3 rounded"><code>[FILE-SPECIFIC CODE]</code></pre>
      <div class="alert alert-info mt-3 mb-0">
        💡 <strong>This Example:</strong> [What this specific file demonstrates]
      </div>
    </div>
  </div>
</div>
```

## Educational Structure

### Required Documentation Cards
Every file must include Purpose and Content cards:

```html
<div class="row justify-content-center mb-4">
  <div class="col-lg-8">
    <div class="card border-0 shadow-sm">
      <div class="card-body">
        <div class="row">
          <div class="col-md-6">
            <h5 class="card-title text-secondary">📚 Purpose</h5>
            <p class="card-text">[Educational objective]</p>
          </div>
          <div class="col-md-6">
            <h5 class="card-title text-secondary">
              🔧 Content | 
              <a href="#format-section" class="text-decoration-none text-info">
                ⚙️ Options API
              </a>
            </h5>
            <p class="card-text">[Technical features]</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
```

### Explanation Sections
Include comprehensive explanation after main demo:

```html
<!-- Vue [Concept] Explanation -->
<div class="mt-4">
  <div class="card border-secondary">
    <div class="card-header bg-secondary text-white">
      <h4 class="card-title mb-0">🔍 How Vue [Concept] Works</h4>
    </div>
    <div class="card-body">
      <ol class="mb-0">
        <li><strong>[Step]:</strong> [Description]</li>
      </ol>
      <div class="row mt-3">
        <div class="col-md-6">
          <div class="alert alert-success mb-0">
            💡 <strong>[Insight]:</strong><br>
            • [Points]
          </div>
        </div>
        <div class="col-md-6">
          <div class="alert alert-info mb-0">
            🎯 <strong>[Pattern]:</strong><br>
            [Description]
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
```

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