
# React Documentation Versioning Policy

React follows a **major-version-centric documentation strategy** to help developers stay aligned with stable API behavior while allowing flexibility across legacy and modern versions.

---

## 📑 Table of Contents

1. [Overview](#overview)
2. [Versioning Policy](#versioning-policy)
3. [Archived Documentation](#archived-documentation)
4. [Legacy Site Structure](#legacy-site-structure)
5. [React 19 Timeline and Expert Summary](#react-19-timeline-and-expert-summary)
    - [React 19 Overview](#react-19-overview)
    - [React v19.0.0 (December 2024)](#react-v1900-december-2024)
    - [React v19.1.0 (March 2025)](#react-v1910-march-2025)
    - [React 19 Expert Summary](#react-19-expert-summary)
<!-- 4. [Expert Summary](#expert-summary) -->
6. [React 18 Timeline and Expert Summary](#react-18-timeline-and-expert-summary)
    - [React 18 Overview](#react-18-overview)
    - [React v18.0.0 (March 2022)](#react-v1800-march-2022)
    - [React v18.1.0 (April 2022)](#react-v1810-april-2022)
    - [React v18.2.0 (June 2022)](#react-v1820-june-2022)
    - [React v18.3.0 (April 2024)](#react-v1830-april-2024)
    - [React v18.3.1 (April 2024)](#react-v1831-april-2024)
    - [React 18 Expert Summary](#react-18-expert-summary)
7. [React 17 Timeline and Expert Summary](#react-17-timeline-and-expert-summary)
    - [React 17 Overview](#react-17-overview)
    - [React v17.0.0 (October 2020)](#react-v1700-october-2020)
    - [React v17.0.1 (October 2020)](#react-v1701-october-2020)
    - [React v17.0.2 (March 2021)](#react-v1702-march-2021)
    - [React 17 Expert Summary](#react-17-expert-summary)
8. [React 16 Timeline and Expert Summary](#react-16-timeline-and-expert-summary)
    - [React 16 Overview](#react-16-overview)
    - [React v16.0 (September 2017)](#react-v160-september-2017)
    - [React v16.1 - v16.2.x](#react-v161---v162x)
    - [React v16.3.x (March - August 2018)](#react-v163x-march---august-2018)
    - [React v16.4 - v16.5.x (May - September 2018)](#react-v164---v165x-may---september-2018)
    - [React v16.6.x (October - November 2018)](#react-v166x-october---november-2018)
    - [React v16.7.0 (December 2018)](#react-v1670-december-2018)
    - [React v16.8.x (February - March 2019)](#react-v168x-february---march-2019)
    - [React v16.9 - v16.10.x (August - October 2019)](#react-v169---v1610x-august---october-2019)
    - [React v16.11 - v16.14.0 (2019 - 2020)](#react-v1611---v16140-2019---2020)
    - [React 16 Expert Summary](#expert-summary)
9. [React 15 Timeline and Expert Summary](#react-15-timeline-and-expert-summary)
    - [React 15 Overview](#react-15-overview)
    - [React v15.0.0 (April 2016)](#react-v1500-april-2016)
    - [React v15.0.1 - v15.0.2](#react-v1501---v1502)
    - [React v15.1.0 (May 2016)](#react-v1510-may-2016)
    - [React v15.2.0 - v15.2.1](#react-v1520---v1521-july-2016)
    - [React v15.3.0 - v15.3.2](#react-v1530---v1532-july-september-2016)
    - [React v15.4.0 - v15.4.2](#react-v1540---v1542-november-2016---january-2017)
    - [React v15.5.0 - v15.5.4](#react-v1550---v1554-april-2017)
    - [React v15.6.0 - v15.6.2](#react-v1560---v1562-june---september-2017)
    - [React v15.7.0 (October 2017)](#react-v1570-october-2017)
    - [React 15 Expert Summary](#react-15-expert-summary)
10. [React 0.14 Timeline and Expert Summary](#react-014-timeline-and-expert-summary)
    - [React 0.14 Overview](#react-014-overview)
    - [React v0.14.0 (October 2015)](#react-v0140-october-2015)
    - [React v0.14.1 (October 2015)](#react-v0141-october-2015)
    - [React v0.14.2 (November 2015)](#react-v0142-november-2015)
    - [React v0.14.3 (November 2015)](#react-v0143-november-2015)
    - [React v0.14.4 (December 2015)](#react-v0144-december-2015)
    - [React v0.14.5 (December 2015)](#react-v0145-december-2015)
    - [React v0.14.6 (January 2016)](#react-v0146-january-2016)
    - [React v0.14.7 (January 2016)](#react-v0147-january-2016)
    - [React v0.14.8 (March 2016)](#react-v0148-march-2016)
    - [React v0.14.10 (October 2020)](#react-v01410-october-2020)
    - [React 0.14 Expert Summary](#react-014-expert-summary)
11. [React 0.13 Timeline and Expert Summary](#react-013-timeline-and-expert-summary)
    - [React 0.13 Overview](#react-013-overview)
    - [React v0.13.0 (March 2015)](#react-v0130-march-2015)
    - [React v0.13.1 (March 2015)](#react-v0131-march-2015)
    - [React v0.13.2 (April 2015)](#react-v0132-april-2015)
    - [React v0.13.3 (May 2015)](#react-v0133-may-2015)
    - [Expert Summary](#expert-summary)

12. [Expert Summary](#expert-summary)


---

## Overview

- The official documentation for the latest React version is hosted at **[react.dev](https://react.dev)**.
- Minor and patch versions are **not separately documented**.
- Documentation is updated **within each major version**.
- Archived docs are accessible via **`x.react.dev`** where `x` is the major version.

---

## Versioning Policy

React publishes updated documentation **only for major releases**:
- Patch and minor version changes are included within the major version’s site.
- When a new major release occurs:
  - The previous version’s documentation is frozen and moved to a subdomain.
  - Example: React 18 docs are archived at `18.react.dev`.

---

## Archived Documentation

| React Version | Documentation URL         |
|---------------|----------------------------|
| 19 (latest)   | [react.dev](https://react.dev)         |
| 18            | [18.react.dev](https://18.react.dev)   |
| 17            | [17.react.dev](https://17.react.dev)   |
| 16            | [16.react.dev](https://16.react.dev)   |
| 15            | [15.react.dev](https://15.react.dev)   |

For versions **older than React 15**, use:
- [15.react.dev](https://15.react.dev)

---

## Legacy Site Structure

- React 18 was the first version with the **new documentation site (react.dev)**.
- Older versions (React 17 and below) use **[legacy.reactjs.org](https://legacy.reactjs.org)**.
- The new site focuses on:
  - Modern features like **hooks**
  - Updated examples
  - Improved navigation and explanations

---



# React 19 Timeline and Expert Summary

React 19 represents the **compiler era** of React. It introduces the **React Compiler (Beta)**, deeper integration of **auto-memoization**, **HTML coordination**, and marks a new phase of performance and DX improvements that reshape how React apps are authored and optimized.

---

## React 19 Overview

React 19 introduces a **source-to-source compiler** that automatically optimizes components. This shift improves render performance and reduces manual `memo` or `useCallback` usage. React also expands **SSR capabilities** and **HTML streaming coordination** to modernize server-rendered workflows.

---

## React v19.0.0 (December 2024)

### Key Features
- **React Compiler (Beta)**:
  - Auto-memoizes components at compile time.
  - Reduces re-renders without manual hooks.
- **HTML Coordination** APIs:
  - More declarative control over markup streaming.
- `use()` hook introduced for streaming async values in Suspense.

### Highlights
- Reduces manual optimization effort.
- Lays groundwork for full concurrent composability.
- Improves Suspense integration with streaming SSR.

### Limitations
- Compiler is opt-in and requires Babel or TypeScript integration.
- Some advanced patterns (refs, closures) may behave differently under the compiler.

### Key Conclusion
- React 19 is about **declarative optimization at scale**, bridging gaps between runtime and compile-time behavior.

---


## React v19.1.0 (March 2025)

### Features
- Stability updates to the React Compiler.
- Expanded Suspense boundary support for SSR fallbacks.
- Better diagnostics and dev mode warnings.

---

## React 19 Expert Summary

React 19 shifts React from a **manual optimization model** to a **compiler-assisted architecture**—changing how performance is achieved in apps.

### 🧠 Why It Matters

- **Compiler-first Design**: Transforms the way React handles reactivity and state change propagation.
- **Suspense Evolution**: With the `use()` hook, asynchronous rendering is more seamless and scalable.
- **SSR Streaming**: HTML coordination improves progressive rendering of server-side React apps.
- **Developer Productivity**: Less need for `useMemo`, `useCallback`, or manual `React.memo`.

React 19 is a strategic leap toward a **more intuitive, performance-automated future**, aligning React with modern expectations for DX and scalability.

---
# React 18 Timeline and Expert Summary

React 18 is a landmark release introducing **Concurrent Rendering**, **automatic batching**, **startTransition**, and major improvements to **Suspense** and **SSR hydration**. It’s a performance-focused version that modernizes React’s runtime while maintaining backward compatibility.


---

## React 18 Overview

React 18 introduced the **Concurrent Renderer**—a new rendering engine that enables React to **pause, interrupt, and resume work**. This allows for smoother UX under heavy computation and dramatically improves scalability for large apps.

---

## React v18.0.0 (March 2022)

### Key Features
- **Concurrent rendering** (opt-in).
- **Automatic batching** for `setState` in async contexts.
- `startTransition()` for low-priority UI updates.
- `useId()` hook for consistent SSR hydration.
- Improved support for `React.lazy()` and `Suspense`.

### Highlights
- Backward-compatible with React 17 apps.
- Required `createRoot()` instead of `ReactDOM.render()` for concurrent features.

---

## React v18.1.0 (April 2022)

- Minor bug fixes and early SSR streaming support improvements.

---

## React v18.2.0 (June 2022)

- Improved hydration resilience.
- Stabilization of `useId` and `startTransition`.
- Updates to automatic batching under complex effects.

---

## React v18.3.0 (April 2024)

- Internal preparations for React 19’s Compiler.
- Better development-mode warnings and debug messages.
- Enhanced Suspense support in edge cases.

---

## React v18.3.1 (April 2024)

- Patch for SSR crash scenarios.
- Miscellaneous fixes related to streaming hydration.
- Developer toolchain improvements.

---

## React 18 Expert Summary

React 18 is the **performance era** of React. It’s engineered for modern apps where rendering should be non-blocking, streaming, and flexible.

### 🧠 Why It Matters

- **Concurrent Mode**: Unlocks features like `Suspense`, `startTransition`, and responsive UI rendering.
- **Automatic Batching**: Reduces unnecessary renders across async boundaries.
- **SSR Hydration**: Faster, more reliable server-side rendering.
- **Transitional APIs**: Maintains full backward compatibility with class and function components.

React 18 makes React **smoother, smarter, and more scalable**—critical for modern apps, SPAs, and streaming platforms.

---

# React 17 Timeline and Expert Summary

React 17 was a **foundational release** with a strong emphasis on **gradual upgrades**, **backward compatibility**, and **modernized event delegation**. While it introduced no new features for the developer API, it laid the infrastructure groundwork for React 18 and beyond.

## React 17 Overview

React 17 focused on **preparing the ecosystem for the future**. It was the first version that allowed **incremental adoption** of future React versions without needing to rewrite entire applications. This was made possible through changes in event delegation, internal refactors, and cleanup of legacy browser behaviors.

---

## React v17.0.0 (October 2020)

### Key Features
- No new developer-facing APIs.
- Modernized event system:
  - Events attached to the **root DOM container** rather than `document`.
- Improved support for concurrent rendering preparation.
- Upgraded error boundaries behavior.

### Highlights
- Enables **embedding multiple React versions** on a single page.
- Compatible with legacy and modern environments simultaneously.
- No need to upgrade all components to use React 17 APIs.

### Limitations
- No features like Suspense improvements or new hooks (those came in React 18).
- Still relies on class components for error boundaries.

### Key Conclusion
- A highly **strategic release**, React 17 focused on **flexibility and stability** across large and legacy codebases.

---

## React v17.0.1 (October 2020)

### Features
- Bug fixes for hydration and event propagation.
- Minor compatibility enhancements for React DOM in edge cases.

---

## React v17.0.2 (March 2021)

### Features
- Further fixes to edge-case hydration mismatches.
- Stability improvements for embedding React within non-React apps.
- Bug fixes for synthetic events and legacy support.

---

## React 17 Expert Summary

React 17 is often called the **“stepping stone release”**. Though it lacked new developer APIs, its **backward-compatible architecture** and **incremental upgrade strategy** made it crucial for teams managing large production apps.

### 🧠 Why It Matters

- **Event Delegation Overhaul**: By moving delegation from `document` to the root container, React became more sandbox-friendly.
- **Incremental Upgrades**: Made it possible to migrate React apps version-by-version—paving the way for React 18's concurrent features.
- **Improved Compatibility**: Allowed embedding or running multiple versions of React on a single page—useful for micro-frontends and hybrid platforms.
- **Zero Feature, Maximum Strategy**: It’s a powerful example of release planning focused on **infrastructure maturity** and **ecosystem readiness**.

React 17 is essential knowledge for any React expert, especially those working in large-scale, enterprise-grade apps requiring long-term maintainability.

---

# React 16 Timeline and Expert Summary

React 16 was a **massive architectural shift** introducing the new **Fiber architecture**, **Error Boundaries**, **Fragments**, and the groundbreaking **Hooks API**. It transformed how developers manage component state, side effects, and render performance.

---

## React 16 Overview

React 16 was a **complete rewrite of React’s core** with the introduction of **Fiber**, a new rendering engine. It enabled interruptible rendering, better error handling, and laid the foundation for hooks, suspense, and concurrent rendering.

---

## React v16.0 (September 2017)

### Key Features
- **Fiber architecture**: asynchronous rendering.
- **Error boundaries** via `componentDidCatch`.
- Return arrays and strings from `render()` (Fragments).
- Portals for rendering outside the DOM hierarchy.

### Highlights
- Massive step forward in performance and stability.
- Fixes for long-standing pain points in rendering logic.

---

## React v16.1 - v16.2.x

- `React.Fragment` short syntax (`<>`) added.
- Improved SSR hydration.
- Miscellaneous bug fixes for the new Fiber internals.

---

## React v16.3.x (March - August 2018)

### Features
- **New Context API** (stable).
- `getDerivedStateFromProps` lifecycle method.
- `createRef()` API for ref management.
- Introduced `forwardRef()` and `React.memo()` (for optimization).

---

## React v16.4 - v16.5.x (May - September 2018)

- Pointer events support added.
- `react-devtools` hooks updated.
- Introduced support for `lazy()` and `Suspense` (code splitting).

---

## React v16.6.x (October - November 2018)

- Introduced `React.lazy()` and `Suspense` officially.
- `contextType` static property added.
- Performance improvements to memoized components.

---

## React v16.7.0 (December 2018)

- **Note**: No hooks yet, but experimental preparation for hooks.

---

## React v16.8.x (February - March 2019)

### 🚨 Key Milestone: React Hooks Introduced

- **useState, useEffect, useContext, useRef, useMemo, useReducer, useCallback**
- Enabled functional components to use state and lifecycle logic.

---

## React v16.9 - v16.10.x (August - October 2019)

- Introduced `act()` testing utility.
- Deprecated legacy string refs.
- Bug fixes in concurrent mode devtools and scheduler.

---

## React v16.11 - v16.14.0 (2019 - 2020)

- Minor improvements to hook behavior.
- `useDeferredValue`, `useTransition` (experimental).
- Improved SSR, `React.lazy()` stabilization.
- `v16.14.0`: compatibility release for React 17 transition.

---

## React 16 Expert Summary

React 16 is one of the most important milestones in React’s evolution. It brought modern rendering paradigms, cutting-edge component ergonomics, and better performance and tooling for large-scale applications.

### 🧠 Why It Matters

- **Fiber Engine**: Enabled concurrent rendering, suspense, and priority-based updates.
- **Hooks**: Removed the need for class components in most use cases.
- **Error Boundaries**: Added production-ready crash resilience.
- **Context API + Memoization**: Better state control and performance in large trees.
- **Modular APIs**: `React.lazy()`, `Suspense`, `forwardRef()` provided clean, optimized composability.

React 16 was more than a version bump—it was a complete rethinking of React's design philosophy.

---

# React 15 Timeline and Expert Summary

React 15 was a crucial step in React’s transition from its early architecture to modern capabilities. It emphasized **render fidelity**, **error boundaries**, and laid important foundations for the upcoming **Fiber architecture** in React 16.

---

## React 15 Overview

React 15 introduced **more accurate rendering**, **HTML attribute normalization**, and **deprecation warnings** for legacy patterns. It also marked the end of support for IE8, allowing cleaner DOM abstraction.

---

## React v15.0.0 (April 2016)

### Key Features
- Split rendering engine into ReactDOM and React Native.
- No more IE8 support.
- Better normalization of SVG and form element attributes.
- `dangerouslySetInnerHTML` safety enhancements.

### Highlights
- Rendering accuracy became a priority.
- Supported cleaner HTML spec-aligned output.

---

## React v15.0.1 - v15.0.2

- Bug fixes and consistency patches around text input fields and attribute merging.

---

## React v15.1.0 (May 2016)

- Added support for custom elements.
- Allowed unknown attributes on DOM nodes.

---

## React v15.2.0 - v15.2.1 (July 2016)

- Introduced PropTypes warnings for invalid props.
- Better handling of whitespace in JSX rendering.

---

## React v15.3.0 - v15.3.2 (July–September 2016)

- Introduced `react-test-renderer`.
- Early preparation for Fiber through internal refactor.
- Improved warnings and memory leak detection.

---

## React v15.4.0 - v15.4.2 (November 2016 – January 2017)

- Separated React and ReactDOM packages for independent upgrades.
- Support for `<details>` and `<summary>` HTML tags.

---

## React v15.5.0 - v15.5.4 (April 2017)

### Key Features
- Moved PropTypes and CreateClass to external packages (`prop-types`, `create-react-class`).
- Start of legacy API deprecation.
- Better dev-only warnings.

---

## React v15.6.0 - v15.6.2 (June – September 2017)

- Improved `onChange` for checkbox/radio inputs.
- Enabled new keyboard event normalization.
- Bug fixes in text selection and controlled inputs.

---

## React v15.7.0 (October 2017)

- Final minor update in 15.x series.
- Contained forward-compatibility fixes for React 16 migration.
- Minor bug cleanup in synthetic event system.

---

## React 15 Expert Summary

React 15 signaled the **last iteration of the classic rendering engine** before Fiber. It emphasized spec-aligned DOM behavior, long-term maintainability, and developer experience.

### 🧠 Why It Matters

- **Deprecation Enforcement**: React 15 began preparing the community for breaking changes by isolating legacy APIs.
- **DOM Compatibility**: HTML5 standards were prioritized.
- **Tooling Enhancements**: The `react-test-renderer` became a vital part of the React testing ecosystem.
- **Performance Awareness**: Paved the way for asynchronous rendering via early internal refactors.

React 15 was a steady, thoughtful evolution of React's internals and developer ergonomics, setting the stage for the groundbreaking React 16.

---

# React 0.14 Timeline and Expert Summary

React 0.14 was a defining release in React's journey toward modularity and scalability. It introduced the **separation of React and ReactDOM**, support for **stateless functional components**, and significant **refinements to component lifecycle management**.

---

## React 0.14 Overview

React 0.14 emphasized architectural modularity and refinement. Its most important change was **splitting React into two packages**: `react` and `react-dom`, paving the way for native rendering engines like **React Native**.

---

## React v0.14.0 (October 2015)

### Key Features
- Split React core into `react` and `react-dom`.
- First-class support for **stateless functional components**.
- New `ReactDOM.findDOMNode` abstraction.
- Composite components can now return arrays of elements.

### Highlights
- Separation of concerns allowed React to scale to multiple renderers.
- Functional components became first-class citizens.

### Limitations
- No built-in memoization or context APIs for functional components.

### Key Conclusion
- Prepared React for extensibility (DOM, Native, VR, etc.) by decoupling rendering logic.

---

## React v0.14.1 (October 2015)

### Features
- Bug fixes for `setState` behavior and warning messages.

### Conclusion
- Minor polish for 0.14.0 rollout.

---

## React v0.14.2 (November 2015)

### Features
- Bug fixes around `dangerouslySetInnerHTML` and invalid prop types.

### Highlights
- Focused on developer safety and spec adherence.

---

## React v0.14.3 (November 2015)

### Features
- Warnings added for invalid JSX nesting.
- Better error boundary fallback support.

---

## React v0.14.4 (December 2015)

### Features
- Fixed class-related inheritance bugs in `React.createClass`.

---

## React v0.14.5 (December 2015)

### Features
- Internal reconciler optimization.
- Better handling of controlled components.

---

## React v0.14.6 (January 2016)

### Features
- Compatibility improvements with React Native.
- Minor SSR bug fixes.

---

## React v0.14.7 (January 2016)

### Features
- Patches for event bubbling and focus delegation.

---

## React v0.14.8 (March 2016)

### Features
- Stability updates and IE9 fixes.

---

## React v0.14.10 (October 2020)

### Features
- Critical security patches applied retroactively.
- No new features; long-term maintenance.

---

## React 0.14 Expert Summary

React 0.14 formalized architectural separation and adopted a more scalable mindset. By enabling stateless components and separating DOM rendering, React set the foundation for:

- **Cross-platform Rendering**: Enabled React Native and custom renderers via `react-dom`, `react-native`, etc.
- **Stateless Components**: Encouraged pure functions over classes when lifecycle/state is not needed.
- **Community Modularity**: Allowed core updates without affecting rendering layers.

### 🧠 Why It Matters

React 0.14 wasn't just about new features — it restructured React to support the ecosystem's explosive growth. With better error messaging, strict mode preparation, and rendering decoupling, React became a flexible and robust platform, not just a library.

---


# React 0.13 Timeline and Expert Summary

React 0.13 marked a major evolution in how developers wrote components. It introduced **ES6 class support**, laid the groundwork for **functional stateless components**, and refined component lifecycles and rendering mechanics.

---

## React 0.13 Overview

React 0.13 introduced **ES6 classes**, **stateless functional components**, and the **new JSX transform**. It was a pivotal step toward modern JavaScript compatibility and better code organization.

---

## React v0.13.0 (March 2015)

### Key Features
- Support for **ES6 class components** using `extends React.Component`.
- Introduced **functional stateless components** (no lifecycle, no state).
- Deprecated `React.createClass` as the primary component definition method.
- Rewritten reconciliation algorithm for better diffing.

### Highlights
- Promoted best practices for maintainability and performance.
- Encouraged adoption of ES6 modules, destructuring, and arrow functions.

### Limitations
- Stateless components lacked `defaultProps` and `propTypes` support natively.
- React.createClass still required for mixins.

### Key Conclusion
- React 0.13 revolutionized component architecture with first-class support for modern JavaScript syntax.

---

## React v0.13.1 (March 2015)

### Key Features
- Bug fixes for new JSX transform.
- Improved error messaging during render failures.

### Highlights
- Stabilized the migration path to ES6 classes and stateless components.

### Limitations
- Bugs when using ES6 class inheritance with custom prototype chains.

### Key Conclusion
- Addressed core edge cases to enable confident adoption of the new patterns.

---

## React v0.13.2 (April 2015)

### Key Features
- Internal enhancements for `React.cloneElement`.
- Fixed incorrect behavior in nested component trees using `refs`.

### Highlights
- Strengthened composition and reuse mechanics.

### Limitations
- Refs still limited to class-based components.

### Key Conclusion
- Improved low-level utilities for advanced patterns.

---

## React v0.13.3 (May 2015)

### Key Features
- Minor bug fixes in server-side rendering scenarios.
- Optimized mounting logic for deeply nested trees.

### Highlights
- Enhanced React’s SSR reliability.

### Limitations
- No full hydration or streaming SSR yet.

### Key Conclusion
- Solidified React 0.13 as a stable base for modern client/server rendering.

---

## Expert Summary

React 0.13 was a transformational release that modernized how React developers architected components. It was the first version to truly embrace JavaScript’s ES6+ syntax and to decouple React from legacy patterns.

### 🧠 Why It Matters

- **ES6 Class Support**: Modern, clean OOP-style components became first-class.
- **Stateless Functional Components**: Lightweight render-only components enabled more performant and declarative UI design.
- **JSX Transform Improvements**: Enabled simpler syntax with less boilerplate.
- **Lifecycle Shift**: Made it easier to think about components as declarative UI factories instead of class instances with mutation.

React 0.13 set the groundwork for everything from **hooks** to **async rendering** by promoting stateless purity and modularity. It remains one of the most important versions in React’s architectural evolution.

---

## Expert Summary

Understanding React’s documentation lifecycle is critical for:
- Maintaining long-lived production systems
- Migrating between major versions
- Accessing accurate legacy behavior (especially pre-hooks/class-based architecture)

### 🧠 Why It Matters

- React emphasizes **stability and long-term support** by maintaining versioned docs.
- React’s versioned documentation enables teams to:
  - Use the right resources for their app’s version.
  - Upgrade incrementally while preserving context-specific references.
  - Avoid confusion between breaking and non-breaking changes.

Always reference the correct subdomain (`x.react.dev`) for historical versions when debugging or planning migrations.

---
