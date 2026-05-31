# 🛠️ CSS Modern Reference & Layout Architect (2026)

A production-grade Claude skill & prompt library aligned with W3C CSS3/4/5 specs, MDN Web Docs, and modern frontend architecture patterns. Built on Eric Meyer's *CSS Pocket Reference* (5th Ed., O'Reilly 2018) and upgraded to 2026 standards.

## 📚 Foundation
This skill is grounded in the authoritative *CSS Pocket Reference* by Eric A. Meyer, providing:
- ✅ Complete selector reference (universal, attribute, pseudo-classes, pseudo-elements)
- ✅ Full property catalog with `Inh.`/`Anim.` flags and formal value syntax
- ✅ Cascade, specificity, and inheritance mechanics explained
- ✅ Box model, layout algorithms (block, inline, flex, grid, table)
- ✅ Value types: colors, lengths, angles, times, URIs, calc(), variables

## 🔄 2026 Modern Upgrades
Beyond the 2018 baseline, this skill adds:
| Feature | Spec Status | Use Case |
|---------|-------------|----------|
| `@layer` cascade control | 🟢 Stable | Architecture precedence management |
| `@scope` & proximity resolution | 🔵 Modern (2024+) | Component-scoped styles |
| `:has()` parent selector | 🟢 Stable | State-driven parent styling |
| Container Queries (`@container`) | 🟢 Stable | Component-responsive layouts |
| Subgrid & Masonry draft | 🔵 Modern | Complex two-dimensional layouts |
| `oklch()`, `color-mix()`, `light-dark()` | 🟢 Stable | Perceptual color & theming |
| Scroll-driven animations | 🔵 Modern | Viewport-based motion |
| `@property` typed custom properties | 🟢 Stable | Animatable CSS variables |
| CSS Nesting (`&`) | 🟢 Stable | Cleaner selector authoring |

## 📦 Quick Start
1. **Clone**: `git clone https://github.com/<your-org>/css-modern-skill.git`
2. **Activate**: Paste `.claude-instructions.md` into Claude's **Custom Instructions** or **Project Settings**
3. **Prompt**: Use `prompts/` templates for rapid debugging & architecture
4. **Context**: Run `@workspace` or `@file styles.css` in Claude Chat for context-aware outputs

## 🧠 Skill Features
- ✅ **Cascade 2.0**: `@layer` → `@scope` → specificity → order resolution
- ✅ **Layout Systems**: Flexbox (`gap`), Grid (`subgrid`), Container Queries, Flow
- ✅ **Modern Selectors**: `:has()`, `:is()`, `:where()`, native nesting (`&`)
- ✅ **Color & Theming**: `oklch()`, `color-mix()`, `light-dark()`, `color-scheme`
- ✅ **Animations**: Scroll timelines, `@property` transitions, view transitions
- ✅ **Progressive Enhancement**: `@supports` fallbacks, browser support tags (🟢/🔵/🟡)

## 📐 Response Framework
Every output follows this spec-compliant structure:


## 🚀 Usage
| Intent | Prompt File | Example Query |
|--------|-------------|---------------|
| Debug cascade conflict | `prompts/cascade-debug.md` | "Why does `.btn:hover` override `@layer components { .btn { ... } }`?" |
| Container query layout | `prompts/container-query.md` | "Build a responsive card with `@container` and fallback" |
| Modern color system | `prompts/modern-color.md` | "Convert `#3B82F6` to `oklch()` + `light-dark()` tokens" |
| Grid architecture | `prompts/layout-architecture.md` | "Design a 3-column dashboard with subgrid + auto-placement" |
| Parent-state styling | `prompts/has-selector.md` | "Style `.form-group` when child `input:invalid` using `:has()`" |
| Scroll animation | `prompts/scroll-timeline.md` | "Implement progress indicator with `animation-timeline: scroll()`" |

## 🗂️ Repository Structure

css-modern-skill/
├── .claude-instructions.md # Core system prompt (drop into Claude)
├── README.md # This file
├── prompts/
│ ├── cascade-debug.md # Specificity & @layer conflict resolver
│ ├── container-query.md # @container component patterns
│ ├── modern-color.md # oklch()/color-mix()/light-dark() theming
│ ├── layout-architecture.md # Grid/Flex/Subgrid patterns
│ └── has-selector.md # :has() parent-state architecture
├── examples/
│ └── skill-output-format.css # Reference implementation of output standards
├── LICENSE # MIT
├── CONTRIBUTING.md # Extension guidelines
└── .gitignore


## 🤝 Contributing
See `CONTRIBUTING.md`. We welcome:
- New prompt templates for emerging CSS features
- Spec updates aligned with W3C Candidate Recommendations
- Architecture patterns for design systems, frameworks, or platforms
- Browser support data refinements (caniuse/MDN cross-references)

### Prompt Guidelines
- Keep prompts under 150 words for clarity
- Always request: cascade impact, fallback strategy, support tags
- Use `${1:placeholder}` syntax for VS Code snippet compatibility
- Test outputs against the Response Framework before submitting

## 📜 License
MIT © Skyconet

---

> 💡 **Pro Tip**: Store `.claude-instructions.md` in your monorepo's `.claude/` folder for auto-detection by AI extensions like Roo Code, Cline, or Continue.dev.