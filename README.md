# CodePilot: AI-Powered VSCode Extension

<div align="center">


   ____          __           ____  _            __
  / __/__  ___  / /________  / __/ (_)__  ___  / /
 _\ \/ _ \/ _ \/ __/ __/ _ \_\ \  / / _ \/ _ \/ / 
/___/\___/\___/\__/_/  \___/___/ /_/\___/_//_/_/  
                                                 


**Your AI-powered copilot for navigating StackOverflow, right inside VSCode.**

</div>

<p align="center">
    <a href="https://github.com/chirag127/CodePilot-AI-Powered-VSCode-Extension/actions/workflows/ci.yml"><img src="https://github.com/chirag127/CodePilot-AI-Powered-VSCode-Extension/actions/workflows/ci.yml/badge.svg?style=flat-square" alt="Build Status"></a>
    <a href="#"><img src="https://img.shields.io/codecov/c/github/chirag127/CodePilot-AI-Powered-VSCode-Extension?style=flat-square" alt="Code Coverage"></a>
    <a href="#"><img src="https://img.shields.io/badge/tech-TypeScript%20%7C%20VSCode%20API-3178C6?style=flat-square" alt="Tech Stack"></a>
    <a href="#"><img src="https://img.shields.io/badge/lint-Biome-56B9F1?style=flat-square" alt="Linter"></a>
    <a href="https://github.com/chirag127/CodePilot-AI-Powered-VSCode-Extension/blob/main/LICENSE"><img src="https://img.shields.io/github/license/chirag127/CodePilot-AI-Powered-VSCode-Extension?style=flat-square&color=blue" alt="License"></a>
    <a href="https://github.com/chirag127/CodePilot-AI-Powered-VSCode-Extension/stargazers"><img src="https://img.shields.io/github/stars/chirag127/CodePilot-AI-Powered-VSCode-Extension?style=social" alt="GitHub stars"></a>
</p>

<p align="center">
  <a href="https://github.com/chirag127/CodePilot-AI-Powered-VSCode-Extension/stargazers"><strong>Star ⭐ this Repo</strong></a> to support the project!
</p>

---

## TL;DR

**CodePilot** is an intelligent VSCode extension that provides real-time, AI-powered code suggestions directly in your editor. It queries StackOverflow and other sources to deliver context-aware completions, accelerating your development workflow without breaking your focus.

## Table of Contents

- [✨ Features](#-features)
- [🏛️ Architecture](#️-architecture)
- [🚀 Getting Started](#-getting-started)
- [🛠️ Development](#️-development)
- [🤖 AI Agent Directives](#-ai-agent-directives)
- [🤝 Contributing](#-contributing)
- [📜 License](#-license)

## ✨ Features

- **Inline Code Suggestions**: Get relevant code snippets based on your current context (comments, function signatures).
- **StackOverflow Integration**: Leverages the vast knowledge base of StackOverflow, parsed and refined by AI.
- **Real-Time Completions**: Suggestions appear as you type, minimizing disruption.
- **Configurable**: Easily toggle features and customize suggestion behavior.
- **Lightweight & Fast**: Optimized for performance to ensure a smooth editor experience.

## 🏛️ Architecture

This project follows a modular, feature-sliced design to ensure scalability and maintainability. Core services are decoupled, allowing for independent testing and development.


.vscode-extension/
├── src/
│   ├── extension.ts        # Main extension entry point
│   ├── services/
│   │   ├── apiService.ts     # Handles StackOverflow/Google queries
│   │   └── completionProvider.ts # Logic for generating suggestions
│   ├── utils/
│   │   └── parser.ts       # HTML/Text parsing utilities
│   └── webview/
│       └── ...               # UI components for settings/display
├── package.json            # Extension manifest and dependencies
└── tsconfig.json           # TypeScript configuration


## 🚀 Getting Started

### Prerequisites

- [Visual Studio Code](https://code.visualstudio.com/) (v1.80.0 or newer)
- [Node.js](https://nodejs.org/) (v18.x or newer)

### Installation

1.  Clone the repository:
    bash
    git clone https://github.com/chirag127/CodePilot-AI-Powered-VSCode-Extension.git
    
2.  Navigate to the project directory:
    bash
    cd CodePilot-AI-Powered-VSCode-Extension
    
3.  Install dependencies:
    bash
    npm install
    
4.  Open the project in VSCode and press `F5` to launch a new Extension Development Host window with the extension activated.

## 🛠️ Development

All development tasks are managed through `npm` scripts defined in `package.json`.

| Script      | Description                                           |
| ----------- | ----------------------------------------------------- |
| `npm run dev`   | Compiles the extension in watch mode for development. |
| `npm run build` | Compiles the extension for production.                |
| `npm run lint`  | Runs Biome to check for linting and format errors.    |
| `npm run test`  | Executes unit and integration tests using Vitest.     |

### Core Principles

- **SOLID**: Each component has a single responsibility, promoting modularity.
- **DRY (Don't Repeat Yourself)**: Reusable utilities and services prevent code duplication.
- **YAGNI (You Ain't Gonna Need It)**: Features are added based on clear requirements, avoiding over-engineering.

---

## 🤖 AI Agent Directives

<details>
<summary><strong>Internal System Directives for AI Development Agents (December 2025 Standard)</strong></summary>

### 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

### 2. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
This repository, `CodePilot-AI-Powered-VSCode-Extension`, is a TypeScript-based developer tool.

*   **PRIMARY SCENARIO: WEB / APP / EXTENSION (TypeScript)**
    *   **Stack:** This project leverages **TypeScript 5.x (Strict Mode)**. Key tools include **WXT (Web Extension Toolkit)** for optimized bundling and cross-browser compatibility, **Biome** for ultra-fast linting and formatting, and **Vitest** for robust unit and integration testing.
    *   **Architecture:** Adheres to **Feature-Sliced Design (FSD)**, ensuring a scalable and maintainable structure with clear boundaries between features, pages, widgets, entities, and shared utilities.
    *   **VSCode API Integration:** Deeply integrated with the VSCode Extension API for core functionalities like inline completions, webviews, and command registration. Prioritize modular design, clear API contracts, and robust error handling for all interactions with the editor's core.
    *   **UI Framework:** For any webview-based UI, use **SolidJS** with **TailwindCSS v4** for its performance and signal-based reactivity model, aligning with 2026 UI trends.

### 3. VERIFICATION & DEPLOYMENT PROTOCOL
*   **Linting & Formatting:** All code **MUST** pass `biome check --apply` before commit. Biome is the Single Source of Truth for code style.
*   **Testing:** All new features **MUST** have >90% unit test coverage via Vitest. E2E tests for critical user flows **MUST** be implemented with Playwright.
*   **CI/CD:** The GitHub Actions workflow (`.github/workflows/ci.yml`) is the gatekeeper. A broken build on `main` is a critical failure. The workflow must run linting, testing, and a production build on every pull request.
*   **API Signatures:** Verify all external API signatures using `docfork`. Do not assume documentation is up-to-date.

</details>

---

## 🤝 Contributing

Contributions are welcome! Please read our [**Contributing Guidelines**](./.github/CONTRIBUTING.md) to get started. We use GitHub Issues for bug reports and feature requests.

## 📜 License

This project is licensed under the [Creative Commons Attribution-NonCommercial 4.0 International License](./LICENSE).
