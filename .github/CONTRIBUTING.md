# 🤝 Contributing to EngageFlow-AI-Social-Reply-Browser-Extension

We welcome contributions to enhance `EngageFlow-AI-Social-Reply-Browser-Extension`. As an Apex-standard repository, we adhere to strict architectural discipline, demanding precision, performance, and future-proofing in all submissions. 

By contributing, you agree that your work will be licensed under **CC BY-NC 4.0**.

## 1. Architectural Alignment (The Apex Standard)

All contributions must align with the core principles detailed in the `AGENTS.md` file. Key architectural mandates include:

*   **SOLID Principles:** Ensure code demonstrates Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion.
*   **DRY & YAGNI:** Avoid needless complexity. Code should solve the immediate problem efficiently without premature generalization.
*   **Technology Stack:** This project is a **JavaScript/TypeScript Browser Extension**. Contributions must maintain strict TypeScript typing (`.ts`/`.tsx`) and leverage modern browser extension APIs (Manifest V3 compliance is mandatory).
*   **Performance Focus:** Browser extension performance is critical. Minimize background processing, optimize DOM manipulation, and ensure rapid API response handling (especially for the Gemini integration).

## 2. Workflow: From Fork to Pull Request

Follow these steps precisely for every contribution:

1.  **Fork the Repository:** Create your own fork of `chirag127/EngageFlow-AI-Social-Reply-Browser-Extension`.
2.  **Clone Locally:** Clone your fork to your development machine.
    bash
    git clone https://github.com/YOUR_USERNAME/EngageFlow-AI-Social-Reply-Browser-Extension.git
    cd EngageFlow-AI-Social-Reply-Browser-Extension
    
3.  **Create a Feature Branch:** Never commit directly to `main` or `develop`.
    bash
    git checkout -b feature/descriptive-branch-name
    
4.  **Develop & Test:** Implement your changes. Crucially, **update or create corresponding unit/integration tests** using Vitest/Playwright.
5.  **Lint & Format:** Before committing, ensure the codebase passes style checks.
    bash
    npm run lint  # Use Biome/ESLint for static analysis
    npm run format # Use Biome for formatting
    
6.  **Commit Atomic Changes:** Write clear, concise commit messages adhering to Conventional Commits specification.
7.  **Push and PR:** Push your branch to your fork and open a Pull Request against `chirag127/EngageFlow-AI-Social-Reply-Browser-Extension:main`.

## 3. Pull Request (PR) Requirements

Every Pull Request must meet the following non-negotiable criteria:

*   **PR Template Completion:** Fill out the provided `PULL_REQUEST_TEMPLATE.md` entirely.
*   **CI/CD Success:** All checks in the `.github/workflows/ci.yml` pipeline **MUST PASS** before a maintainer will review the code.
*   **Coverage Threshold:** Ensure no new code introduces coverage gaps. Target a minimum of **90% test coverage** for new features.
*   **Contextual Description:** Clearly articulate *why* the change is necessary and *how* it affects the system architecture.

## 4. Reporting Issues and Security Vulnerabilities

### Bug Reports
Use the predefined template (`.github/ISSUE_TEMPLATE/bug_report.md`) when reporting bugs. Provide clear steps to reproduce, expected vs. actual behavior, and relevant environment details (OS, Browser Version).

### Security Vulnerabilities

**DO NOT** report security vulnerabilities publicly. We adhere to a strict responsible disclosure policy. Please follow the guidelines in `.github/SECURITY.md` and contact us privately via email or GitHub Security Advisory.

--- 

*Thank you for investing your expertise in elevating `EngageFlow-AI-Social-Reply-Browser-Extension`.*