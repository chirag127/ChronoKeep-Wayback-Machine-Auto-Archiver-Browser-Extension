# ChronoKeep-Wayback-Machine-Auto-Archiver-Browser-Extension

A browser extension that automatically preserves your digital footprint by saving every visited webpage to the Internet Archive's Wayback Machine. Features a customizable ignore list for privacy and security.

[![Build Status](https://img.shields.io/github/actions/workflow/user/chirag127/ChronoKeep-Wayback-Machine-Auto-Archiver-Browser-Extension/ci.yml?style=flat-square)](https://github.com/chirag127/ChronoKeep-Wayback-Machine-Auto-Archiver-Browser-Extension/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/ChronoKeep-Wayback-Machine-Auto-Archiver-Browser-Extension?style=flat-square)](https://codecov.io/gh/chirag127/ChronoKeep-Wayback-Machine-Auto-Archiver-Browser-Extension)
[![Tech Stack](https://img.shields.io/badge/tech-stack-TypeScript%2C%20Vite%2C%20TailwindCSS%2C%20Tauri-blue?style=flat-square)](https://github.com/chirag127/ChronoKeep-Wayback-Machine-Auto-Archiver-Browser-Extension)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-orange?style=flat-square)](https://github.com/chirag127/ChronoKeep-Wayback-Machine-Auto-Archiver-Browser-Extension/blob/main/LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/ChronoKeep-Wayback-Machine-Auto-Archiver-Browser-Extension?style=flat-square)](https://github.com/chirag127/ChronoKeep-Wayback-Machine-Auto-Archiver-Browser-Extension)

**Star ⭐ this Repo**

---

## 🚀 Project Overview

ChronoKeep is an intelligent browser extension designed for passive digital preservation. It automatically archives every webpage you visit to the Internet Archive's Wayback Machine, ensuring your browsing history is durably recorded. With advanced customization options, including a per-site ignore list, you maintain complete control over what gets archived, prioritizing privacy and security.

---

## 🏗️ Architecture

mermaid
graph TD
    A[User Browsing Activity] --> B{ChronoKeep Extension}
    B --> C{URL Filtering & Ignore List Check}
    C -- Archive --> D[Web Archive API Call (Wayback Machine)]
    C -- Ignore --> E[No Action]
    D --> F[Archived Page on Wayback Machine]
    E --> G[Browser Continues]


---

## 📚 Table of Contents

*   [🚀 Project Overview](#-project-overview)
*   [🏗️ Architecture](#️-architecture)
*   [🌟 Key Features](#-key-features)
*   [🛠️ Technology Stack](#️-technology-stack)
*   [⚙️ Installation & Setup](#-installation--setup)
*   [🔧 Usage](#-usage)
*   [📝 AI Agent Directives](#-ai-agent-directives)
*   [🤝 Contributing](#-contributing)
*   [📜 License](#-license)

---

## 🌟 Key Features

*   **Automatic Archiving:** Seamlessly saves every visited page to the Wayback Machine.
*   **Customizable Ignore List:** Define specific websites or URL patterns to exclude from archiving, respecting your privacy.
*   **Real-time Feedback:** Visual indicators show when a page has been successfully archived.
*   **Cross-Browser Support:** Built for Chrome and Firefox.
*   **Lightweight & Efficient:** Minimal performance impact on your browsing experience.

---

## 🛠️ Technology Stack

*   **Language:** TypeScript (Strict Mode)
*   **Build Tool:** Vite 7 (Rolldown)
*   **UI Framework:** TailwindCSS v4
*   **Native Integration:** Tauri v2.x
*   **Architecture:** Feature-Sliced Design (FSD) principles adapted for extensions.
*   **State Management:** Signals (Standardized)
*   **Linting/Formatting:** Biome
*   **Testing:** Vitest (Unit) & Playwright (E2E)

---

## ⚙️ Installation & Setup

Follow these steps to set up ChronoKeep locally:

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/ChronoKeep-Wayback-Machine-Auto-Archiver-Browser-Extension.git
    cd ChronoKeep-Wayback-Machine-Auto-Archiver-Browser-Extension
    

2.  **Install Dependencies:**
    bash
    npm install
    

3.  **Build the Extension:**
    bash
    npm run build
    

4.  **Load Unpacked Extension:**
    *   **Chrome:** Go to `chrome://extensions/`, enable Developer Mode, click "Load unpacked", and select the `dist` or `build` folder.
    *   **Firefox:** Go to `about:debugging#/runtime/this-firefox`, click "Load Temporary Add-on", and select the `manifest.json` file from the `dist` or `build` folder.

---

## 🔧 Usage

Once installed, ChronoKeep operates automatically in the background. Visit `chrome://extensions/` (or `about:debugging`) to manage its settings, including configuring the ignore list.

---

## 📝 AI Agent Directives

<details>
<summary><strong>View AI Agent Directives</strong></summary>

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
**Directives:** Detect the project type and apply the corresponding **Apex Toolchain**.

*   **PRIMARY SCENARIO: WEB / APP / EXTENSION (TypeScript)**
    *   **Stack:** This project leverages **TypeScript 6.x (Strict Mode)**. Key tools include **Vite 7** (for building and development server), **Tauri v2.x** (for native integration), and **WXT** (for modern extension development). Use **Biome** for ultra-fast linting and formatting, and **Vitest** for unit testing, supplemented by **Playwright** for end-to-end testing.
    *   **Architecture:** Adheres to **Feature-Sliced Design (FSD)**, ensuring modularity, scalability, and maintainability. Maintain clear separation of concerns for UI, business logic, and platform-specific interactions.
    *   **State Management:** Employ **Signals** (standardized approach) for efficient and reactive state updates across the extension.
    *   **Styling:** Utilize **TailwindCSS v4** for rapid and consistent UI development.

*   **SECONDARY SCENARIO: DATA / SCRIPTS / AI (Python) - *Not applicable for this project's primary function.***
    *   **Stack:** uv (Manager), Ruff (Linter), Pytest (Test).
    *   **Architecture:** Modular Monolith or Microservices.

---

## 4. VERIFICATION COMMANDS

*   **Lint & Format:**
    bash
    npm run lint
    npm run format
    

*   **Unit Tests:**
    bash
    npm run test:unit
    

*   **End-to-End Tests:**
    bash
    npm run test:e2e
    

*   **Build:**
    bash
    npm run build
    

---

## 5. ARCHITECTURAL PRINCIPLES

*   **SOLID:** Apply all five principles to ensure maintainable and scalable code.
*   **DRY (Don't Repeat Yourself):** Eliminate redundant code and logic.
*   **YAGNI (You Ain't Gonna Need It):** Implement only necessary features.
*   **Feature-Sliced Design (FSD):** Maintain strict modularity and clear boundaries between features, layers, and segments.

---

## 6. SECURITY PROTOCOL

*   **Dependency Scanning:** Regularly scan dependencies for vulnerabilities using `npm audit` or equivalent tools.
*   **API Key Management:** Securely manage any API keys or sensitive credentials (e.g., using environment variables, `.env` files with `dotenv`, or Tauri's secure storage mechanisms). **NEVER** hardcode secrets.
*   **Input Validation:** Rigorously validate all user inputs and external data to prevent injection attacks.
*   **Content Security Policy (CSP):** Implement strict CSP headers if applicable (e.g., in Tauri's `tauri.conf.json`).
*   **Privacy by Design:** Ensure user privacy is paramount. Minimize data collection and clearly document all data handling practices.

</details>

---

## 🤝 Contributing

Contributions are welcome! Please refer to the [.github/CONTRIBUTING.md](/.github/CONTRIBUTING.md) file for detailed guidelines on how to contribute to this project.

---

## 📜 License

This project is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0). See the [LICENSE](LICENSE) file for more details.
