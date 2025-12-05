<div align="center">

<img src="https://raw.githubusercontent.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/main/.github/assets/banner.png" alt="CodeInsight Banner">

# CodeInsight: AI Code Assistant VSCode Extension

</div>

<div align="center">

[
![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/ci.yml?branch=main&style=flat-square)
](https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/actions/workflows/ci.yml)
[
![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension?style=flat-square&token=CODECOV_TOKEN)
](https://codecov.io/gh/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension)
[
![Tech Stack](https://img.shields.io/badge/tech-TypeScript_|_VSCode_API-blue?style=flat-square)
](https://www.typescriptlang.org/)
[
![Linter](https://img.shields.io/badge/lint-Biome-blueviolet?style=flat-square)
](https://biomejs.dev/)
[
![License](https://img.shields.io/github/license/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension?style=flat-square)
](https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/blob/main/LICENSE)
[
![GitHub Stars](https://img.shields.io/github/stars/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension?style=flat-square)
](https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/stargazers)

</div>

> **CodeInsight** is an AI-powered VSCode extension that provides real-time, context-aware code suggestions by leveraging the vast knowledge base of StackOverflow. Supercharge your development workflow and solve coding challenges instantly, directly within your editor.

<div align="center">
<a href="https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/stargazers"> 
    <img src="https://img.shields.io/static/v1?label=Star&message=this%20Repo&color=blue&style=for-the-badge&logo=github" alt="Star this Repo"/>
</a>
</div>

---

## 📋 Table of Contents

- [✨ Key Features](#-key-features)
- [🏛️ Architecture Overview](#️-architecture-overview)
- [🚀 Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [🛠️ Development Scripts](#️-development-scripts)
- [🤖 AI Agent Directives (2026 Standard)](#-ai-agent-directives-2026-standard)
- [🤝 Contributing](#-contributing)
- [📜 License](#-license)

---

## ✨ Key Features

- **Real-Time IntelliSense:** Get intelligent code completions sourced directly from relevant StackOverflow answers.
- **Context-Aware Snippets:** Suggestions are tailored to your current file type, frameworks, and code context.
- **In-Editor Documentation:** View explanations and usage examples without ever leaving your IDE.
- **Productivity Boost:** Reduce time spent searching for solutions and accelerate your development cycle.
- **Seamless Integration:** Works effortlessly within the native VSCode environment.

---

## 🏛️ Architecture Overview

This extension follows the **Feature-Sliced Design (FSD)** pattern for a scalable and maintainable codebase. This ensures a clear separation of concerns and simplifies the process of adding new features.

plaintext
.vscode/
src/
├── extension.ts          # Main extension entry point & command registration
├── core/
│   ├── api/              # API clients (e.g., StackOverflow)
│   ├── cache/            # Caching layer for API responses
│   └── state.ts          # Global extension state management
├── features/
│   ├── get-code-completion/ # Logic for providing code completions
│   └── show-hover-docs/     # Logic for displaying documentation on hover
├── shared/
│   ├── lib/              # Reusable helper functions & utilities
│   ├── types/            # Global TypeScript types and interfaces
│   └── constants.ts      # Shared constants
└── test/                 # Vitest test suites
    ├── suite/
    │   ├── extension.test.ts
    │   └── index.ts
    └── runTest.ts
package.json


---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v20.x or higher)
- [Visual Studio Code](https://code.visualstudio.com/)

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension.git
    cd CodeInsight-AI-Code-Assistant-VSCode-Extension
    

2.  **Install dependencies:**
    bash
    npm install
    

3.  **Run the extension:**
    - Open the project in VSCode.
    - Press `F5` to open a new Extension Development Host window with the extension loaded.

---

## 🛠️ Development Scripts

| Script      | Description                                                 |
| ----------- | ----------------------------------------------------------- |
| `npm run vscode:prepublish` | Compiles the TypeScript code before publishing.             |
| `npm run compile`           | Compiles the project without watching for changes.          |
| `npm run watch`             | Compiles and watches for file changes.                      |
| `npm run lint`              | Lints and formats the codebase using Biome.                 |
| `npm run test`              | Runs the unit and integration tests using Vitest.           |

---

## 🤖 AI Agent Directives (2026 Standard)

<details>
<summary>Expand for AI Agent Instructions</summary>

<br>

# SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

## 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

---

## 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat this `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

---

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** This repository, `CodeInsight-AI-Code-Assistant-VSCode-Extension`, is a TypeScript-based VSCode Extension.

*   **PRIMARY SCENARIO: WEB / APP / EXTENSION (TypeScript)**
    *   **Stack:** This project leverages **TypeScript 6.x (Strict)**. Key tools include **Biome** (for ultra-fast linting and formatting), **Vitest** (for unit/integration testing), and the native **VSCode API** (`vscode`). Bundling is handled by `esbuild` via the `vsce` CLI.
    *   **Architecture:** Adheres to **Feature-Sliced Design (FSD)**. This modular pattern ensures a clean separation of concerns, isolating features like `code-completion` and `hover-documentation` into self-contained slices. This simplifies maintenance and scales effectively.
    *   **AI Integration:** The core AI logic involves querying the **StackOverflow API**. Future enhancements should focus on using a vector embedding model (e.g., from Hugging Face or OpenAI) to perform semantic searches on a pre-indexed dataset of StackOverflow answers for superior contextual relevance.
    *   **State Management:** Utilizes VSCode's native state management APIs (`context.globalState`, `context.workspaceState`) for persistence.
    *   **Verification Commands:**
        *   Linting & Formatting: `npm run lint`
        *   Testing: `npm run test`
        *   Type Checking: `npm run compile`

*   **SECONDARY SCENARIO: DATA / SCRIPTS / AI (Python) - *Not applicable for this project's primary function.***
    *   Reference only for potential future backend services or data processing pipelines.

</details>

---

## 🤝 Contributing

Contributions are welcome! Please see our [Contributing Guidelines](https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/blob/main/.github/CONTRIBUTING.md) for more details on how to get involved.

---

## 📜 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License**. See the [LICENSE](https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/blob/main/LICENSE) file for details.
