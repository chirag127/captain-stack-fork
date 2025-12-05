# Contributing to CodeInsight-AI-Code-Assistant-VSCode-Extension

Thank you for considering contributing to the **CodeInsight AI Code Assistant VSCode Extension**! We aim to maintain a high-velocity, zero-defect development process. To ensure consistency and quality across all contributions, please adhere to the following guidelines.

## 1. Code of Conduct

This project adheres to the Contributor Covenant Code of Conduct. Please read the [Code of Conduct](https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/blob/main/CODE_OF_CONDUCT.md) to understand the expected standards of behavior.

## 2. Development Environment Setup (Late 2025 Standards)

Our extension is built using **TypeScript 6.x (Strict)** and leverages **Vite 7 (Rolldown)** for building and bundling. **WXT (Web Extension Tooling)** is used for managing the extension lifecycle across different browsers. **Biome** is employed for linting and formatting, and **Vitest** for unit testing.

Follow these steps to set up your development environment:

1.  **Clone the Repository:**
    bash
    git clone https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension.git
    cd CodeInsight-AI-Code-Assistant-VSCode-Extension
    

2.  **Install Dependencies:**
    We use `npm` as our package manager. Ensure you have Node.js 20+ installed.
    bash
    npm install
    

3.  **Build the Extension:**
    bash
    npm run dev
    
    This command will build the extension in watch mode, suitable for development.

4.  **Run Tests:**
    bash
    npm test
    
    This command runs all unit tests using Vitest.

5.  **Lint and Format Code:**
    We use Biome for code quality. Run the following commands:
    bash
    # Check and fix linting and formatting issues
    npm run lint -- --fix
    # Or just check without fixing
    npm run lint
    

## 3. Contribution Workflow

We follow a standard GitHub pull request workflow:

1.  **Fork the Repository:** Create your own fork of the `chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension` repository.

2.  **Create a New Branch:** Branch out from the `main` branch for your feature or bug fix.
    bash
    git checkout -b feature/your-feature-name
    

3.  **Make Your Changes:** Implement your changes, ensuring they follow the project's coding standards and architectural principles (SOLID, DRY, YAGNI).

4.  **Test Your Changes:** Write comprehensive unit tests for any new functionality or bug fixes. Ensure all existing tests pass.

5.  **Lint and Format:** Run `npm run lint -- --fix` to ensure your code adheres to the project's formatting and linting standards.

6.  **Commit Your Changes:** Write clear and concise commit messages.
    bash
    git add .
    git commit -m "feat: Add descriptive commit message"
    

7.  **Push to Your Fork:** Push your changes to your fork on GitHub.
    bash
    git push origin feature/your-feature-name
    

8.  **Open a Pull Request:** Open a pull request from your feature branch to the `main` branch of the `chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension` repository.

    *   **PR Template:** Ensure your pull request description follows the [Pull Request Template](https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/blob/main/.github/PULL_REQUEST_TEMPLATE.md).

## 4. Architectural Principles

We adhere to the following principles:

*   **SOLID:** Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, Dependency Inversion.
*   **DRY:** Don't Repeat Yourself.
*   **YAGNI:** You Ain't Gonna Need It.
*   **Feature-Sliced Design (FSD):** For frontend/extension architecture, we aim for a clear separation of concerns into features, layers, and segments.

## 5. Code Submission Standards

*   **TypeScript Strict Mode:** All TypeScript code must be written with `strict: true` enabled in `tsconfig.json`.
*   **Linter:** Biome will automatically catch most style and potential code issues. Ensure it passes without errors or warnings.
*   **Tests:** All new code must be accompanied by relevant unit tests.
*   **Documentation:** Update relevant documentation (e.g., `README.md`, inline comments) as needed.

## 6. Reporting Issues

Before reporting an issue, please check if it already exists. If not, please use the [Bug Report Issue Template](https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/blob/main/.github/ISSUE_TEMPLATE/bug_report.md) to provide detailed information.

## 7. Security Vulnerabilities

If you discover a security vulnerability, please follow our [Security Policy](https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/blob/main/.github/SECURITY.md) for reporting.

## 8. AI Agent Directives

This repository is managed by Apex AI Agents. Ensure your contributions align with the directives outlined in the [AGENTS.md](https://github.com/chirag127/CodeInsight-AI-Code-Assistant-VSCode-Extension/blob/main/AGENTS.md) file. Key aspects include:

*   **Tech Stack:** TypeScript 6.x (Strict), Vite 7, WXT, Biome, Vitest.
*   **Architecture:** Feature-Sliced Design (FSD).
*   **Verification:** Use `npm test` for unit tests and `npm run lint` for code quality checks.
*   **AI Integration:** Context-aware code suggestions leveraging StackOverflow data. Ensure API integrations are robust and efficient.

---*

*By contributing, you agree to abide by these guidelines and the project's Code of Conduct.*