# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview
This is a Vue.js learning project containing standalone HTML files that demonstrate various Vue 3 concepts and features. Each file is a self-contained example that can be opened directly in a browser.

## Architecture
- **Standalone HTML files**: Each example is a complete HTML document with embedded Vue.js code
- **Vue 3 ES Module**: Uses `vue.esm-browser-3-3-4.js` imported as ES module
- **No build process**: Files run directly in the browser without compilation
- **Bootstrap 5**: Several examples use Bootstrap for styling
- **Local assets**: Images stored in `img/` directory

## Key Files Structure
- `vue_1_einbinden.html` - Basic Vue integration and expression evaluation
- `vue_2_evaluate_expression.html` - Mathematical expressions in templates
- `vue_3_input_field_and_databinding.html` - Two-way data binding with v-model
- `vue_4_use_conditional_evaluation.html` - Conditional rendering
- `vue_5_show_image_databinding_bootstrap.html` - Image display with Bootstrap
- `vue_5b_show_images_databinding_method.html` - Image display with methods
- `vue_6_use_mounted_hook.html` - Component lifecycle hooks
- `vue_7_add_image.html` - Dynamic image addition with user input
- `vue_7_iterate_with_v-for.html` - List rendering with v-for directive

## Development Workflow
- Open HTML files directly in browser to view examples
- No build, test, or compilation commands needed
- Each file demonstrates specific Vue 3 concepts in isolation
- German comments and UI text throughout codebase

## Vue 3 Patterns Used
- ES module imports from local Vue file
- Composition API with `createApp()`
- Data function returning objects for reactivity
- Template directives: v-model, v-for, v-on (@), :src, :style
- Event handling with methods
- Bootstrap integration for responsive layouts

## File Naming Convention
Files follow pattern: `vue_[number]_[description].html` with progressive complexity and feature introduction.