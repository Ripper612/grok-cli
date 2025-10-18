# Grok CLI Hurry Mode

## Project Overview

This is a command-line tool that brings a conversational AI assistant, powered by the Grok API, into the terminal. It is a Node.js project written in TypeScript.

The tool provides an interactive chat interface for interacting with the AI, as well as a headless mode for scripting and automation. It has a rich set of features, including:

*   **Advanced File Operations:** Editing, creating, and reading files.
*   **Code Intelligence:** Abstract Syntax Tree (AST) parsing, symbol search, and dependency analysis for multiple languages.
*   **Web Interaction:** Fetching content from URLs and performing web searches.
*   **Task Management:** A system for managing tasks and to-do lists.
*   **Extensibility:** Support for Model Context Protocol (MCP) servers to add custom tools.

The user interface is built with Ink, a React renderer for command-line applications.

## Building and Running

### Prerequisites

*   Node.js 18+

### Installation and Execution

1.  **Install dependencies:**
    ```bash
    npm install
    ```

2.  **Build the project:**
    ```bash
    npm run build
    ```

3.  **Run in development mode:**
    ```bash
    npm run dev
    ```

4.  **Run the production build:**
    ```bash
    npm start
    ```

5.  **Global command:**
    The main command to run the CLI is `grok`.

### Available Scripts

*   `npm run build`: Compiles the TypeScript code using `tsup`.
*   `npm run dev`: Builds the project and runs the CLI in development mode.
*   `npm start`: Executes the compiled CLI.
*   `npm run lint`: Lints the codebase using ESLint.
*   `npm run typecheck`: Performs a TypeScript type check.

## Development Conventions

*   **Language:** TypeScript
*   **Code Style:** The project uses ESLint for linting, with configurations in `eslint.config.mjs`.
*   **Pre-commit Hooks:** Husky is used to run linting and type checks before each commit to maintain code quality.
*   **Automated Releases:** The project has a fully automated release system using GitHub Actions. Every push to the `main` branch triggers a new version bump, build, and npm publication.
*   **AI Agent Documentation:** The `.agent` directory contains a comprehensive set of documents outlining the architecture, standard operating procedures (SOPs), and tasks for an AI agent working on this project. This suggests that the project is designed to be developed and maintained with the help of AI.
*   **Configuration:** The project uses a `.grok` directory for user and project-specific settings, including API keys and model preferences.
