
# React Documentation Versioning Policy

React follows a **major-version-centric documentation strategy** to help developers stay aligned with stable API behavior while allowing flexibility across legacy and modern versions.

---

## 📑 Table of Contents

1. [Overview](#overview)
2. [Versioning Policy](#versioning-policy)
3. [Archived Documentation](#archived-documentation)
4. [Legacy Site Structure](#legacy-site-structure)
5. [Expert Summary](#expert-summary)

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
