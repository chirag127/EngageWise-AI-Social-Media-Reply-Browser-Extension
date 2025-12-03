# Contributing to EngageWise-AI-Social-Media-Reply-Browser-Extension

Thank you for considering contributing to **EngageWise-AI-Social-Media-Reply-Browser-Extension**! Your efforts help make this project better for everyone.

This project adheres to the Apex Technical Authority standards, emphasizing **Zero-Defect, High-Velocity, Future-Proof** development.

## 1. Code of Conduct

This project and its contributors are bound by the Contributor Covenant Code of Conduct. Please ensure your contributions are respectful and inclusive.

- [Contributor Covenant Code of Conduct v2.0](https://www.contributor-covenant.org/version/2/0/CODE_OF_CONDUCT.html)

## 2. Getting Started

Before you start contributing, please ensure you have the necessary development environment set up.

### 2.1 Prerequisites

*   **Node.js:** v20 or later (check `.nvmrc` for the exact version).
*   **npm / Yarn / pnpm:** Package manager.
*   **Git:** For version control.

### 2.2 Setup

1.  **Fork the repository:** Click the "Fork" button on the GitHub repository page.
2.  **Clone your fork:**
    bash
    git clone https://github.com/chirag127/EngageWise-AI-Social-Media-Reply-Browser-Extension.git
    cd EngageWise-AI-Social-Media-Reply-Browser-Extension
    
3.  **Install dependencies:**
    bash
    npm install
    # or yarn install, or pnpm install
    

### 2.3 Branching Strategy

*   All development should occur on feature branches. Do not commit directly to `main`.
*   Branch names should be descriptive and follow the pattern: `feat/your-feature-name`, `fix/your-bug-fix`, `chore/maintenance-task`.

## 3. Contribution Workflow

1.  **Find an issue to work on:** You can find open issues [here](https://github.com/chirag127/EngageWise-AI-Social-Media-Reply-Browser-Extension/issues).
2.  **Create a new branch:** Based on your issue, create a descriptive branch.
    bash
    git checkout -b feat/add-new-platform-support
    
3.  **Make your changes:** Implement your feature or fix.
4.  **Test your changes:** Ensure all tests pass and add new tests if necessary.
    bash
    npm run test
    
5.  **Lint and format your code:**
    bash
    npm run lint
    npm run format
    
6.  **Commit your changes:** Write clear and concise commit messages.
    bash
    git commit -m "feat: Add support for new platform XYZ"
    
7.  **Push your branch:**
    bash
    git push origin feat/add-new-platform-support
    
8.  **Open a Pull Request:** Go to your fork on GitHub and create a Pull Request to the `main` branch of the `chirag127/EngageWise-AI-Social-Media-Reply-Browser-Extension` repository.

## 4. Pull Request Guidelines

*   **Descriptive Title and Description:** Clearly explain the purpose of your PR and the changes made.
*   **Link to Issue:** Reference the relevant issue in your PR description (e.g., `Fixes #123`).
*   **Code Reviews:** Be responsive to feedback from maintainers.
*   **CI Checks:** Ensure all continuous integration checks pass before merging.

## 5. Development Standards & Architecture

This project follows the Apex Technical Authority's standards:

*   **Technology Stack:** TypeScript (Strict), Vite, TailwindCSS v4, Tauri v2. (Note: As this is a browser extension, the Tauri v2 mention might be aspirational or for a desktop wrapper. Core focus remains on web technologies.)
*   **Linting & Formatting:** Biome (Speed) + Vitest (Unit) + Playwright (E2E).
*   **Architecture:** Feature-Sliced Design (FSD) principles are encouraged for maintainability and scalability.
*   **AI Integration:** Leverages AI models for context-aware reply generation. Ensure API keys are managed securely (e.g., via environment variables or secrets management) and not committed to the repository.
*   **Principles:** Adhere to SOLID, DRY, and YAGNI principles.

## 6. Reporting Issues

If you find a bug or have a feature request, please open an issue on the GitHub repository.

*   **Bug Reports:** Provide a clear description of the bug, steps to reproduce it, expected behavior, and actual behavior. Include relevant environment details.
*   **Feature Requests:** Describe the feature you envision and explain why it would be beneficial.

## 7. Contact

If you have any questions not covered here, feel free to reach out to the maintainer(s) via GitHub Issues.

Thank you for contributing!
