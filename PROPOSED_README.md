# EngageWise: AI-Powered Social Media Reply Assistant Browser Extension

![Build Status](https://img.shields.io/github/actions/workflow/user/chirag127/EngageWise-AI-Social-Media-Reply-Browser-Extension/ci.yml?style=flat-square)
![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/EngageWise-AI-Social-Media-Reply-Browser-Extension?style=flat-square)
![Tech Stack](https://img.shields.io/badge/Tech%20Stack-JavaScript%2C%20WebExtensions%2C%20AI-blue?style=flat-square)
![Lint/Format](https://img.shields.io/badge/Linter%20%26%20Formatter-Biome-FF1493?style=flat-square)
![License](https://img.shields.io/github/license/chirag127/EngageWise-AI-Social-Media-Reply-Browser-Extension?color=orange&style=flat-square)
![GitHub Stars](https://img.shields.io/github/stars/chirag127/EngageWise-AI-Social-Media-Reply-Browser-Extension?style=flat-square)

[//]: <> (Link to copy this repo to your GitHub account)
<a href="https://github.com/chirag127/EngageWise-AI-Social-Media-Reply-Browser-Extension/generate" target="_blank"><img src="https://user-images.githubusercontent.com/334831/142823707-55958f18-0876-40e1-8b6e-4b168a6e491c.png" width="150" alt="Use This Template"></a>

## Overview

EngageWise is an intelligent browser extension that leverages advanced AI to craft context-aware and tone-adjusted replies across major social media platforms like X, LinkedIn, and Reddit. Enhance your online engagement and brand presence with AI-driven assistance.

## Architecture

mermaid
graph TD
    A[Browser Extension Host] --> B{Content Script};
    B --> C[Platform DOM Interaction];
    B --> D[AI Service API];
    D --> E(AI Model - Text Generation);
    E --> D;
    D --> B;
    B --> F[Background Script];
    F --> G[Storage API];
    F --> H[User Options UI];
    H --> F;
    G --> F;


## Table of Contents

*   [Overview](#overview)
*   [Architecture](#architecture)
*   [Table of Contents](#table-of-contents)
*   [AI Agent Directives](#ai-agent-directives)
*   [Development Standards](#development-standards)
*   [Setup](#setup)
*   [Scripts](#scripts)
*   [Contributing](#contributing)
*   [License](#license)

<details>
<summary>🤖 AI Agent Directives</summary>

## AI Agent Directives: EngageWise

This section outlines the core directives and technical specifications for AI agents interacting with the EngageWise project. Adherence ensures maximum compatibility and leverages the full potential of the Apex Architecture.

### 1. Core Philosophy & Identity

*   **Role:** Senior Principal Software Architect & Master Technical Copywriter (40+ years experience).
*   **Prime Directive:** "Zero-Defect, High-Velocity, Future-Proof."
*   **Standard:** FAANG-level precision.

### 2. Project Context & Stack (December 2025 Standard)

*   **Repository Name:** `EngageWise-AI-Social-Media-Reply-Browser-Extension`
*   **Primary Language:** JavaScript (ES2023+)
*   **Frameworks/Libraries:** WebExtensions API, Vite (Bundler), Biome (Linter/Formatter).
*   **Target Platforms:** Chrome, Firefox, Edge (via WebExtensions).
*   **AI Integration:** Utilizes external AI APIs for context-aware reply generation. Prioritize modularity, clear API contracts, and robust error handling.

### 3. Architectural Patterns

*   **Frontend:** Adheres to modern web extension patterns, separating concerns between content scripts (DOM manipulation, UI injection) and background scripts (event handling, API communication, state management).
*   **Code Quality:** Enforces **SOLID** principles, **DRY** (Don't Repeat Yourself), and **YAGNI** (You Ain't Gonna Need It). Rigorous adherence to Biome for code style and linting.

### 4. Verification & Testing Commands

*   **Linting & Formatting:** `npm run lint` (or `biome check --apply`)
*   **Unit Testing:** `npm run test:unit` (using Vitest or Jest)
*   **E2E Testing:** `npm run test:e2e` (using Playwright)
*   **Build:** `npm run build`

### 5. Data Handling & Security

*   **API Keys:** Never hardcode API keys. Utilize secure storage mechanisms provided by the browser or environment variables during development.
*   **User Data:** Handle all user data with utmost privacy and security. Comply with all relevant data protection regulations.

### 6. Documentation Standards

*   **README:** Must be comprehensive, detailing setup, usage, architecture, and contribution guidelines.
*   **AGENTS.md:** This document serves as the source of truth for AI agent interaction.
*   **Code Comments:** Essential for complex logic, non-obvious implementations, and API interactions.

--- JDH/142823707 ---
</details>

## Development Standards

This project adheres to the following principles to ensure maintainability, scalability, and robustness:

*   **SOLID Principles:** (Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, Dependency Inversion) applied rigorously to all modules.
*   **DRY (Don't Repeat Yourself):** Minimize code duplication through abstraction and modular design.
*   **YAGNI (You Ain't Gonna Need It):** Implement only the necessary features, avoiding premature optimization or speculative design.
*   **Immutability:** Prefer immutable data structures where applicable to prevent unexpected side effects.
*   **Strict Typing:** Utilize TypeScript (or JavaScript with JSDoc for strictness) to catch errors at compile time.

## Setup

Follow these steps to set up the development environment:

1.  **Clone the Repository:**
    bash
    git clone https://github.com/chirag127/EngageWise-AI-Social-Media-Reply-Browser-Extension.git
    cd EngageWise-AI-Social-Media-Reply-Browser-Extension
    

2.  **Install Dependencies:**
    bash
    npm install
    

3.  **Environment Variables:**
    Create a `.env` file in the root directory and add your AI service API keys:
    env
    VITE_AI_API_KEY=your_api_key_here
    VITE_AI_API_ENDPOINT=your_api_endpoint_here
    

4.  **Load Extension in Browser:**
    *   **Chrome/Edge:** Open `chrome://extensions/` or `edge://extensions/`, enable "Developer mode," click "Load unpacked," and select the `dist` folder (or the root folder if building locally).
    *   **Firefox:** Open `about:debugging#/runtime/this-firefox`, click "Load Temporary Add-on," and select any file within the project directory.

## Scripts

| Script                | Description                                                      |
| :-------------------- | :--------------------------------------------------------------- |
| `npm run dev`         | Runs the Vite dev server for local development.                  |
| `npm run build`       | Builds the production-ready extension files into the `dist` folder. |
| `npm run lint`        | Lints and formats code using Biome.                              |
| `npm run test:unit`   | Runs unit tests using Vitest.                                    |
| `npm run test:e2e`    | Runs end-to-end tests using Playwright.                          |
| `npm run preview`     | Previews the production build locally.                           |

## Contributing

Contributions are welcome! Please refer to the [.github/CONTRIBUTING.md](/.github/CONTRIBUTING.md) file for detailed guidelines.

## License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** license. See the [LICENSE](LICENSE) file for more details.
