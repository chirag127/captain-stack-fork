# 🚀 Contribution Guidelines for CodePilot-AI-Powered-VSCode-Extension

Welcome to the Apex project! As a steward of this codebase, we adhere to the **Apex Technical Authority** standards: Zero-Defect, High-Velocity, and Future-Proof development. Contributions are the lifeblood of evolution; your rigorous attention to detail is expected and appreciated.

## 1. Guiding Philosophy

Before contributing, internalize the core directives found in `.github/AGENTS.md`. This repository operates under strict architectural patterns (SOLID, DRY) and leverages TypeScript 6.x, Vite 7, and the Biome tooling suite for maximum performance and maintainability.

## 2. The Contribution Workflow

All contributions must follow this standardized path:

1.  **Fork:** Create a personal fork of the `main` branch.
2.  **Clone:** Clone your fork locally: `git clone https://github.com/YOUR_USERNAME/CodePilot-AI-Powered-VSCode-Extension.git`
3.  **Branching:** Create a new feature branch for your work. **Naming Convention:** `feat/short-description`, `fix/issue-number`, or `refactor/area-name`.
    bash
git checkout -b feat/ai-model-caching

4.  **Development & Testing (Crucial Step):**
    *   Implement your changes, adhering strictly to the **TypeScript Strict Mode**.
    *   **Verification Commands:** Before committing, ensure all quality gates pass. For this VSCode extension, use the following command suite:
        bash
        # Install dependencies (using uv if applicable, though Node/npm is standard for TS)
        npm install
        
        # Run Linter/Formatter Check (Biome)
        npm run lint
        npm run format:check

        # Run Unit Tests (Vitest)
        npm test

        # Run E2E/Integration Tests (Playwright)
        npm run test:e2e
        
5.  **Commit:** Write atomic, clear, and descriptive commit messages following the Conventional Commits specification.
6.  **Push:** Push your branch to your fork: `git push origin feat/ai-model-caching`
7.  **Pull Request (PR):** Open a Pull Request against `chirag127:main`.

## 3. Pull Request Requirements

Every PR MUST reference the associated issue (if applicable) and must adhere to the template in `.github/PULL_REQUEST_TEMPLATE.md`.

*   **Mandatory Checklist:**
    *   [ ] Code passes all `npm run lint` checks.
    *   [ ] All associated unit tests pass (`npm test`).
    *   [ ] Functional changes include new or updated documentation.
    *   [ ] Architectural adherence (SOLID, DRY) has been maintained or improved.

## 4. Security Disclosures

We treat security with the highest priority. If you discover a security vulnerability, **DO NOT** open a public issue. Follow the protocol outlined in `.github/SECURITY.md` for responsible disclosure.

## 5. Code Style and Standards

*   **Language:** TypeScript (Strict configuration enforced).
*   **Tooling:** Biome is the exclusive tool for linting and formatting. Configure your editor to utilize Biome presets.
*   **Architecture:** Prefer clear interfaces and dependency injection patterns (where applicable for extension architecture) to maintain modularity.
*   **Naming:** All variables, functions, and classes must be descriptively named. Avoid single-letter variables unless standard (e.g., loop counters `i`, `j`).

--- 

*Thank you for elevating this project. Your adherence to these standards ensures the longevity and stability of the CodePilot ecosystem.*