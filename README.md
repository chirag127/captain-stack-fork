<p align="center">
  <img src="https://raw.githubusercontent.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/main/.github/assets/logo.png" alt="CodeInsight Logo" width="200"/>
</p>

<h1 align="center">CodeInsight-AI-Code-Assistant-VSCode-Extension</h1>

<p align="center">
  <a href="https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/actions/workflows/ci.yml">
    <img src="https://img.shields.io/github/actions/workflow/status/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/ci.yml?branch=main&style=flat-square&label=Build%20Status" alt="Build Status">
  </a>
  <a href="https://codecov.io/gh/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension">
    <img src="https://img.shields.io/codecov/c/github/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension?style=flat-square&label=Coverage" alt="Code Coverage">
  </a>
  <img src="https://img.shields.io/badge/Tech%20Stack-TypeScript%20%7C%20WXT%20%7C%20Vite%20%7C%20VSCode-blueviolet?style=flat-square" alt="Tech Stack">
  <img src="https://img.shields.io/badge/Lint%2FFmt-Biome-9D721A?style=flat-square" alt="Lint/Format: Biome">
  <a href="https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey?style=flat-square" alt="License: CC BY-NC 4.0">
  </a>
  <a href="https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/stargazers">
    <img src="https://img.shields.io/github/stars/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension?style=flat-square&label=Stars&color=fcc624" alt="GitHub Stars">
  </a>
</p>

<p align="center">
  Star ⭐ this Repo to show your support and help our project grow!
</p>

---

## 🚀 Overview: AI-Powered Code Assistance for VSCode

CodeInsight-AI-Code-Assistant-VSCode-Extension is an intelligent VSCode extension that revolutionizes developer productivity by providing real-time, context-aware code suggestions directly within your editor. Leveraging advanced AI, it analyzes your codebase and current context to deliver precise completions, bug fixes, and best-practice recommendations, significantly reducing development time and improving code quality.

This extension taps into a vast knowledge base, including insights from platforms like StackOverflow, to offer highly relevant and accurate suggestions. It's designed to seamlessly integrate into your existing workflow, acting as a proactive coding companion that understands your intent and helps you write better code faster.

---

## 🎯 Key Features

*   **Real-time AI Suggestions:** Context-aware code completions and recommendations as you type.
*   **StackOverflow Integration:** Harnesses community knowledge for problem-solving and best practices.
*   **Intelligent Refactoring:** Suggests optimal code structure and improvements.
*   **Error Detection & Fixes:** Proactively identifies potential issues and offers solutions.
*   **Customizable Experience:** Tailor AI models and suggestion preferences to your needs.
*   **Seamless VSCode Integration:** Works natively within your favorite editor environment.

---

## 🏗️ Architecture

CodeInsight employs a robust, modular architecture designed for performance, extensibility, and maintainability, following the **Feature-Sliced Design (FSD)** principles.

mermaid
graph TD
    A[VSCode Editor] -->|Communicates via LSP| B(Extension Host)
    B --> C{Core Extension Logic}
    C --> D[Language Server Client]
    D --> E[Language Server (Node.js)]
    E --> F[AI API Service]
    E --> G[Context Analyzer]
    E --> H[StackOverflow API]

    F --&gt;|AI Suggestions| E
    G --&gt;|Code Context| E
    H --&gt;|Community Data| E
    C --&gt;|Manages Webviews| I[UI Components (Webviews)]
    I --&gt;|User Interaction| A


**Key Components:**

*   **Extension Host:** The main entry point for the VSCode extension, managing activation, commands, and communication with the Language Server Client.
*   **Language Server Client:** Facilitates communication between the VSCode extension and the Language Server via the Language Server Protocol (LSP).
*   **Language Server (Node.js):** The core backend service responsible for processing code, generating suggestions, and interacting with external services. It analyzes the AST, provides diagnostics, and serves completions.
*   **Context Analyzer:** Extracts relevant code snippets, surrounding syntax, and project structure to provide rich context for the AI model.
*   **AI API Service:** Interfaces with external AI models (e.g., Google Gemini, OpenAI GPT) to generate intelligent code suggestions, refactoring ideas, and error fixes based on the provided context.
*   **StackOverflow API Integration:** Queries and parses StackOverflow data to incorporate community-driven solutions and best practices into suggestions.
*   **UI Components (Webviews):** Interactive web-based interfaces within VSCode for settings, detailed explanations, or custom suggestion UIs.

---

## ⚙️ Installation & Setup

To get CodeInsight running in your VSCode environment:

1.  **Clone the Repository:**
    bash
    git clone https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension.git
    cd CodeInsight-AI-Code-Assistant-VSCode-Extension
    

2.  **Install Dependencies:**
    bash
    npm install
    

3.  **Build the Extension:**
    bash
    npm run build
    

4.  **Run in Development Mode:**
    *   Open the project folder in VSCode.
    *   Press `F5` to open a new VSCode window with the extension loaded.

5.  **Install from VSIX (for production release):**
    *   Generate the `.vsix` file: `npm run package`
    *   In VSCode, open the Command Palette (`Ctrl+Shift+P` or `Cmd+Shift+P`), type `Extensions: Install from VSIX...`, and select the generated `.vsix` file.

---

## 🚀 Development Scripts

This project uses `npm` scripts for common development tasks:

| Script          | Description                                                    |
| :-------------- | :------------------------------------------------------------- |
| `npm run dev`   | Starts the development server for watch mode and debugging.    |
| `npm run build` | Compiles the TypeScript code into JavaScript for production.   |
| `npm test`      | Runs unit and integration tests with Vitest.                   |
| `npm run e2e`   | Executes end-to-end tests using Playwright.                    |
| `npm run lint`  | Lints the codebase using Biome for code quality and style.     |
| `npm run format`| Formats the codebase using Biome.                              |
| `npm run package`| Packages the extension into a `.vsix` file for distribution. |
| `npm run watch` | Watches for changes and recompiles (for specific scenarios).   |

---

## 🤖 AI Agent Directives

<details>
<summary><b>🔥 AGENT OPERATIONAL MANDATE 🔥</b></summary>
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
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

---

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type and apply the corresponding **Apex Toolchain**. This repository, `CodeInsight-AI-Code-Assistant-VSCode-Extension`, is a TypeScript-based VSCode extension with AI capabilities.

*   **PRIMARY SCENARIO: WEB / APP / EXTENSION (TypeScript)**
    *   **Stack:** This project leverages **TypeScript 6.x (Strict)** for robust type safety, **Vite 7** with `Rolldown` for blazing-fast development and optimized builds, and **WXT** (Web eXtension Toolkit) for streamlined VSCode extension development.
    *   **Architecture:** Adheres to the **Feature-Sliced Design (FSD)** pattern, ensuring clear module boundaries, scalable feature development, and maintainable codebase. Components are organized by feature, layer, and slice.
    *   **State Management:** Utilizes **Signals** (e.g., Preact Signals, Solid.js Signals) for efficient and reactive state management within webviews and UI components.
    *   **Lint/Format:** **Biome** is used for ultra-fast and comprehensive linting, formatting, and auto-fixing, ensuring code consistency and quality.
    *   **Testing:** **Vitest** for blazing-fast unit and component testing, and **Playwright** for robust end-to-end (E2E) testing of extension functionality within VSCode.
    *   **AI Integration:** Deeply integrated with **Google Gemini API** (`gemini-3-pro` by default) or similar LLM providers (configurable) for intelligent code suggestions, context analysis, and refactoring recommendations. Prioritize modular design, clear API contracts, and robust error handling for all AI model interactions.

*   **SECONDARY SCENARIO B: SYSTEMS / PERFORMANCE (Rust/Go) - *Not applicable for this project. Reference only.***
    *   **Stack:** Rust (Cargo) or Go (Modules).
    *   **Lint:** Clippy / GolangCI-Lint.
    *   **Architecture:** Hexagonal Architecture (Ports & Adapters).

*   **SECONDARY SCENARIO C: DATA / AI / SCRIPTS (Python) - *Not applicable for this project. Reference only.***
    *   **Stack:** uv (Manager), Ruff (Linter), Pytest (Test).
    *   **Architecture:** Modular Monolith or Microservices.
</details>

---

## 📖 Principles & Guidelines

This project adheres to the following core software development principles:

*   **SOLID Principles:**
    *   **S**ingle Responsibility Principle
    *   **O**pen/Closed Principle
    *   **L**iskov Substitution Principle
    *   **I**nterface Segregation Principle
    *   **D**ependency Inversion Principle
*   **DRY (Don't Repeat Yourself):** Avoid redundancy by abstracting common functionalities.
*   **YAGNI (You Aren't Gonna Need It):** Implement features only when they are actually needed.
*   **Clean Code:** Prioritize readability, maintainability, and extensibility.
*   **Test-Driven Development (TDD):** Write tests before implementing features to ensure robust and verifiable code.

---

## 🤝 Contributing

We welcome contributions! Please refer to our [Contributing Guidelines](.github/CONTRIBUTING.md) for details on how to get started.

---

## 🛡️ Security

For information on security practices and how to report vulnerabilities, please see our [Security Policy](.github/SECURITY.md).

---

## 📄 License

This project is licensed under the [Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0) License](LICENSE).
