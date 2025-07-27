# T032: Vue API Markers and Format Sections

## Objective
Add Vue API identification to all learning files for educational clarity and future categorization.

## Implementation Design

### API Visual System
- **Options API**: ⚙️ icon (gear represents configuration/options approach)
- **Future Composition API**: 🧩 icon (puzzle piece represents composable functions)

### Integration Method
**Content Card Title Enhancement:**
```html
<!-- Current -->
<h5 class="card-title text-secondary">🔧 Content</h5>

<!-- Enhanced -->
<h5 class="card-title text-secondary">
  🔧 Content | 
  <a href="#format-section" class="text-decoration-none text-info">
    ⚙️ Options API
  </a>
</h5>
```

### Format Section Addition
**File-specific format sections** - each file shows its actual Vue structure:

#### vue_1_einbinden.html Example:
```html
<div id="format-section" class="card border-info">
  <div class="card-header bg-info text-white">
    <h4 class="card-title mb-0">⚙️ Vue Options API Format</h4>
  </div>
  <div class="card-body">
    <pre class="bg-light p-3 rounded"><code>createApp().mount('#app');</code></pre>
    <div class="alert alert-info mt-3 mb-0">
      💡 <strong>This Example:</strong> Basic Vue integration and mounting without data or methods.
    </div>
  </div>
</div>
```

#### vue_6_use_mounted_hook.html Example:
```html
<div id="format-section" class="card border-info">
  <div class="card-header bg-info text-white">
    <h4 class="card-title mb-0">⚙️ Vue Options API Format</h4>
  </div>
  <div class="card-body">
    <pre class="bg-light p-3 rounded"><code>createApp({
  data() {
    return { imgURLs: [...], index: 0 }
  },
  methods: {
    previous() { /* navigation */ },
    next() { /* navigation */ }
  },
  mounted() {
    setInterval(this.next, 5000);
  }
}).mount('#app');</code></pre>
    <div class="alert alert-info mt-3 mb-0">
      💡 <strong>This Example:</strong> Lifecycle hooks with automatic timers and navigation methods.
    </div>
  </div>
</div>
```

### File-Specific Approach
Each format section must show:
1. **Actual code structure** used in that specific file
2. **Relevant explanation** of what that structure demonstrates
3. **Educational progression** from simple to complex

## Files to Update

### Implementation Progress

#### Completed Files ✅
- `vue_1_einbinden.html` - Basic mounting only
- `vue_6_use_mounted_hook.html` - Lifecycle hooks with timers

#### Remaining Files (T032g)
1. `vue_1b_cdn_integration.html` - CDN approach with global Vue object
2. `vue_2_evaluate_expression.html` - Data with calculations
3. `vue_3_input_field_and_databinding.html` - Data + methods with v-model
4. `vue_4_use_conditional_evaluation.html` - Data with conditional logic
5. `vue_4b_conditional_directives.html` - Data + methods with directives
6. `vue_5_show_image_databinding_bootstrap.html` - Data with attribute binding
7. `vue_5b_show_images_databinding_method.html` - Data + methods for navigation
8. `vue_7_dynamic_content_addition.html` - Data + methods for dynamic arrays
9. `vue_7_iterate_with_v-for.html` - Data + methods with v-for iteration

#### Specific Format Examples for Remaining Files

**vue_1b_cdn_integration.html:**
```javascript
const { createApp } = Vue;
createApp({ 
  data() { return { message: 'Hello from CDN!' } },
  methods: { updateMessage() {...} }
}).mount('#app');
```
*This Example: CDN integration with global Vue object approach.*

**vue_2_evaluate_expression.html:**
```javascript
createApp({
  data() { return { x: 25, y: 14 } }
}).mount('#app');
```
*This Example: Template expressions with reactive calculations.*

**vue_3_input_field_and_databinding.html:**
```javascript
createApp({
  data() { return { x: 25, y: 14 } },
  methods: {
    setExampleValues() {...},
    resetValues() {...}
  }
}).mount('#app');
```
*This Example: Two-way data binding with user input and programmatic updates.*

## Benefits
- **Educational Clarity**: Students understand which Vue approach they're learning
- **Future Expansion**: Ready for Composition API examples
- **Professional Presentation**: Clear technical documentation
- **Navigation**: Quick access to API format reference
- **Consistency**: Uniform approach across all learning files

## Implementation Status - COMPLETED ✅

### All Tasks Completed (2025-07-27)
- [x] ✅ DEVELOPER_GUIDE.md created with comprehensive standards
- [x] ✅ STYLE_GUIDE.md updated with API marker requirements  
- [x] ✅ Planning document updated for file-specific approach
- [x] ✅ All 10 vue files updated with ⚙️ Options API markers
- [x] ✅ All files have file-specific format sections with relevant code examples
- [x] ✅ All format sections include educational explanations
- [x] ✅ Anchor linking implemented (#format-section)
- [x] ✅ Consistent Bootstrap styling applied

### Files Completed
1. ✅ vue_1_einbinden.html - Basic mounting
2. ✅ vue_1b_cdn_integration.html - CDN with global Vue object
3. ✅ vue_2_evaluate_expression.html - Data with calculations
4. ✅ vue_3_input_field_and_databinding.html - Data + methods with v-model
5. ✅ vue_4_use_conditional_evaluation.html - Data with validation logic
6. ✅ vue_4b_conditional_directives.html - Data + methods with directives
7. ✅ vue_5_show_image_databinding_bootstrap.html - Data with attribute binding
8. ✅ vue_5b_show_images_databinding_method.html - Data + methods for navigation
9. ✅ vue_6_use_mounted_hook.html - Lifecycle hooks with timers
10. ✅ vue_7_dynamic_content_addition.html - Dynamic arrays with manipulation
11. ✅ vue_7_iterate_with_v-for.html - List rendering with selection

## Technical Notes
- Use `text-decoration-none text-info` for clean link styling
- Maintain existing Bootstrap color scheme (info theme)
- Ensure `#format-section` anchor linking works properly
- Keep format examples concise but representative of actual file content
- Position format section after main explanation for logical flow
- Each format section must be unique and educational