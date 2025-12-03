# EngageWise-AI-Social-Media-Reply-Browser-Extension

![Build Status](https://img.shields.io/github/actions/workflow/user/chirag127/EngageWise-AI-Social-Media-Reply-Browser-Extension/ci.yml?style=flat-square&logo=githubactions)
![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/EngageWise-AI-Social-Media-Reply-Browser-Extension?style=flat-square&logo=codecov)
![Tech Stack](https://img.shields.io/badge/Tech%20Stack-JS%7CVite%7CTailwindCSS%7CTauri-blue?style=flat-square)
![Linting](https://img.shields.io/badge/Lint%2FFormat-Biome-purple?style=flat-square)
![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgray?style=flat-square)
![GitHub Stars](https://img.shields.io/github/stars/chirag127/EngageWise-AI-Social-Media-Reply-Browser-Extension?style=flat-square&logo=github)

[⭐ Star this Repo ⭐](https://github.com/chirag127/EngageWise-AI-Social-Media-Reply-Browser-Extension)

---


**EngageWise** is an intelligent browser extension designed to revolutionize your social media interactions. By leveraging advanced AI, it generates context-aware and tone-adjusted replies across platforms like X, LinkedIn, and Reddit, significantly enhancing your engagement and productivity.

---


## Architecture Overview

mermaid
graph TD
    A[Browser Extension Core] --> B(UI Layer: Content Scripts/Popup)
    A --> C(Background Scripts: Event Handling/API Calls)
    C --> D{AI Service Integration}
    D -- Contextual Data --> E[LLM API (e.g., OpenAI, Gemini)]
    E -- Generated Reply --> D
    D -- Formatted Reply --> C
    C -- Display/Post --> B
    B -- User Interaction --> A
    A --> F(Local Storage/State Management)


---


## Table of Contents

*   [Features](#features)
*   [AI Agent Directives](#ai-agent-directives)
*   [Technology Stack](#technology-stack)
*   [Development Setup](#development-setup)
*   [Project Structure](#project-structure)
*   [Contribution Guidelines](#contribution-guidelines)
*   [License](#license)

---


## Features

*   **AI-Powered Reply Generation:** Generates relevant and context-specific replies for social media posts.
*   **Tone Adjustment:** Adapts reply tone (professional, casual, witty, etc.) to match user preference and platform context.
*   **Cross-Platform Support:** Works seamlessly on X, LinkedIn, Reddit, and potentially other platforms.
*   **Context Awareness:** Analyzes the original post and conversation history to craft intelligent responses.
*   **Productivity Boost:** Saves time by automating the drafting of replies.
*   **Lightweight & Efficient:** Built with modern web technologies for optimal performance.

---


## AI Agent Directives

<details>
<summary>Click to expand AI Agent Directives</summary>

### SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

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
**Directives:** Detect the project type and apply the **Apex Toolchain**.

*   **PRIMARY SCENARIO A: WEB / APP / EXTENSION (TypeScript)**
    *   **Stack:** TypeScript 6.x (Strict), Vite 7 (Rolldown), Tauri v2.x (Native), WXT (Extensions framework for Vite). 
    *   **State Management:** Employ standardized Signals for robust and efficient state handling across the extension.
    *   **UI Framework:** Tailwind CSS v4 for utility-first styling.
    *   **Linting/Formatting:** Biome (latest stable version) for superior performance and comprehensive code quality checks.
    *   **Testing:** Vitest for unit/integration testing, Playwright for end-to-end (E2E) testing.
    *   **Architecture:** Feature-Sliced Design (FSD) principles for maintainable and scalable extension architecture.
    *   **AI Integration:** Focus on efficient background scripting and content script communication for AI model interactions (e.g., external APIs like OpenAI, Gemini).

---

## 4. APEX NAMING CONVENTION (THE "STAR VELOCITY" ENGINE)
**Formula:** `<Product-Name>-<Primary-Function>-<Platform>-<Type>`
**Format:** `Title-Case-With-Hyphens`
**Rules:**
1.  **Length:** 3 to 10 words.
2.  **Keywords:** MUST include high-volume terms.
3.  **Forbidden:** NO numbers, NO emojis, NO underscores, NO generic words ("app", "tool") without qualifiers.
4.  **Archival Protocol:** If `action` is "ARCHIVE", you MUST still generate a new name, description, and topics.

---

## 5. CODING STANDARDS & BEST PRACTICES
*   **TypeScript:** STRICTLY use `strict: true` mode.
*   **Reusability:** Adhere to DRY (Don't Repeat Yourself) and KISS (Keep It Simple, Stupid) principles.
*   **Modularity:** Design components and modules for maximum reusability and testability.
*   **Error Handling:** Implement robust error handling, especially for external API calls and AI interactions.
*   **Security:** Sanitize all user inputs and API payloads. Be mindful of XSS vulnerabilities in extensions.
*   **Performance:** Optimize for speed and memory usage, especially in background and content scripts.

---

## 6. TESTING & VERIFICATION PROTOCOL
*   **Unit Tests:** Comprehensive unit tests using Vitest, covering individual functions and components.
*   **Integration Tests:** Verify interactions between different modules and services.
*   **E2E Tests:** End-to-end testing with Playwright to simulate real user scenarios within the browser environment.
*   **Code Coverage:** Aim for >85% code coverage. Use Codecov for reporting.

---

## 7. VERIFICATION COMMANDS
*   **Install Dependencies:** `npm install` or `yarn install`
*   **Run Development Server (Vite):** `npm run dev` or `yarn dev`
*   **Build Extension:** `npm run build` or `yarn build`
*   **Run Linter/Formatter:** `npx @biomejs/biome check --apply .`
*   **Run Unit Tests:** `npx vitest run`
*   **Run E2E Tests:** `npx playwright test`

</details>

---


## Technology Stack

*   **Language:** JavaScript (ESNext)
*   **Framework:** Vite 7 (for build and development server)
*   **Runtime:** Tauri v2.x (for native packaging and browser integration)
*   **UI Styling:** Tailwind CSS v4
*   **Linting & Formatting:** Biome
*   **Testing:** Vitest (Unit/Integration), Playwright (E2E)
*   **AI:** Integration with external LLM APIs (e.g., OpenAI, Gemini)

---


## Development Setup

Follow these steps to set up the development environment:

1.  **Clone the Repository:**
    bash
    git clone https://github.com/chirag127/EngageWise-AI-Social-Media-Reply-Browser-Extension.git
    cd EngageWise-AI-Social-Media-Reply-Browser-Extension
    

2.  **Install Dependencies:**
    bash
    npm install
    # or if you prefer yarn:
    # yarn install
    

3.  **Set up Environment Variables (if applicable):**
    Create a `.env` file in the root directory and add necessary API keys (e.g., `VITE_OPENAI_API_KEY`). Consult the `.env.example` file for structure.

4.  **Run in Development Mode:**
    bash
    npm run dev
    # or
    # yarn dev
    
    This will start the Vite development server and allow you to load the extension in your browser (instructions for loading unpacked extensions can be found in your browser's developer documentation).

5.  **Run Linter and Formatter:**
    Ensure code quality and consistency:
    bash
    npx @biomejs/biome check --apply .
    

6.  **Run Tests:**
    Execute unit and E2E tests:
    bash
    # Run unit tests
    npx vitest run

    # Run E2E tests
    npx playwright test
    

---


## Project Structure


EngageWise-AI-Social-Media-Reply-Browser-Extension/
├── public/
│   └── logo.png
├── src/
│   ├── background/
│   │   └── index.ts
│   ├── content/
│   │   └── index.ts
│   ├── ui/
│   │   ├── components/
│   │   ├── pages/
│   │   └── main.ts
│   ├── assets/
│   ├── constants.ts
│   ├── utils.ts
│   └── types.ts
├── index.html
├── manifest.json
├── tsconfig.json
├── vite.config.ts
├── README.md
├── LICENSE
├── .gitignore
├── package.json
└── ... other config files


---


## Contribution Guidelines

We welcome contributions! Please refer to the [CONTRIBUTING.md](https://github.com/chirag127/EngageWise-AI-Social-Media-Reply-Browser-Extension/blob/main/.github/CONTRIBUTING.md) file for detailed information on how to submit pull requests, report bugs, and suggest features.

---


## License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)**. See the [LICENSE](https://github.com/chirag127/EngageWise-AI-Social-Media-Reply-Browser-Extension/blob/main/LICENSE) file for more details.
