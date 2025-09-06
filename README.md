# PolyChronos Ω — An AI-Powered Software Development Framework

**Orchestrate a guild of AI savants to build enterprise-grade software. PolyChronos Ω is a comprehensive, persona-driven framework that brings strategic discipline, quality assurance, and intelligent automation to your development workflow in Cursor.**

---

This repository is more than a project scaffold; it's a complete operating system for modern software development. By leveraging a **persona-driven**, **phase-aware**, and **context-first** methodology, it transforms your IDE into a coordinated team of AI experts ready to architect, build, and deliver exceptional software.

---

## ✨ Key Features

-   **Expert Guild of Personas**: Work with a team of specialized AI savants, ensuring every task is handled by an expert with the right skills and mindset.
-   **Structured Planning Templates**: Utilize a comprehensive set of Markdown templates (`PRD`, `Architecture`, `TestPlan`) to build a deep, shared context for the AI.
-   **Phase-Gated Workflow**: Progress through the software development lifecycle with explicit quality gates, ensuring discipline and preventing costly mistakes.
-   **Customizable Quality Rules**: Define your project's engineering standards for code, testing, and security directly in the `.cursorrules` file.
-   **Seamless Cursor Integration**: Designed from the ground up to leverage Cursor's unique features like `@file` context and custom system prompts.

---

## 🎭 Meet the Guild: A Few Key Personas

PolyChronos comes with a full team of AI savants. Here are the core leaders you'll be working with:

#### Strategic & Leadership
-   🔭 **Visionary Planner**: Your strategic guide who identifies market opportunities and defines the project's North Star.
-   🗺️ **Product Strategist**: The voice of the user, translating their needs into a prioritized roadmap and actionable stories.
-   🎯 **Project Manager**: The master orchestrator who creates clarity, manages risk, and keeps the project moving with momentum.
-   📜 **The Loremaster**: The guardian of the project's knowledge, who transforms scattered information into a single, clear source of truth.

#### Architectural & Engineering
-   🏛️ **Savant Architect**: The holistic system architect who designs the high-level blueprint, ensuring all components (front end, back end, AI) fit together perfectly.
-   🎨 **Front End Architect & Designer**: The master artist of the user experience, who crafts beautiful, intuitive, and bleeding-edge interfaces.
-   ⚙️ **Back End Architect & Designer**: The master engineer of the system's core, who builds the powerful, scalable, and reliable server-side foundation.
-   🧠 **Nexus Architect**: The AI genius who architects emergent intelligence and autonomous agentic systems.
-   🛡️ **The Sentinel (Security Engineer)**: The guardian of trust who proactively engineers security into every layer of the project.
-   👷 **Lead Engineer**: The hands-on craftsperson who leads the implementation of the architecture and mentors the engineering team.

---

## 🏛️ The PolyChronos Philosophy

-   **Persona-Driven**: Every task is handled by an AI expert with the specific skills and mindset for the job. You're not just prompting an AI; you're collaborating with a specialist.
-   **Phase-Aware**: The framework understands the software development lifecycle. It guides you from discovery and planning through to deployment and maintenance with structured phases.
-   **Context-First**: AIs are only as good as their context. Our templates are designed to build a rich, multi-layered understanding of your project, ensuring the AI's outputs are deeply relevant and intelligent.

---

## 🚀 Your First Project Workflow

Follow these steps to initialize the framework and begin your first project. **The Loremaster** persona will facilitate this documentation process, ensuring your project's knowledge base is built on a solid foundation from the very start.

1.  **Clone the Repository**: Start by cloning this project scaffold into your local workspace.
    ```bash
    git clone [your-repo-url]
    ```
2.  **Complete the Discovery Document**: Begin by filling out `/docs/living/Discovery.md`. This captures the high-level business case and validates the opportunity.
3.  **Define the Product with the PRD**: With the discovery validated, complete the `/docs/living/PRD.md`. This defines *what* you're building and *why*.
4.  **Architect the Solution**: Based on the PRD, fill out the `/docs/living/Architecture.md`. This is a collaborative effort led by the **Savant Architect** and validated by **The Sentinel**, with crucial input from the **Front End** and **Back End** specialists.
5.  **Configure Project Rules**: Open `.cursorrules` and adjust any settings, like the default persona or code quality thresholds, to fit your needs.
6.  **Activate PolyChronos**: In Cursor, set the contents of `/.cursor/prompts/PolyChronos-Omega.md` as your project's system prompt.
7.  **Engage the Project Manager**: The AI `Project Manager` will now activate, review your completed templates, and begin orchestrating the build. Advance through phases using the **👍 `Proceed`** command when prompted.

---

## 🗂️ Project Structure

The repository is organized to clearly separate context, documentation, and prompts.

```bash
.
├── .cursor/
│   └── prompts/
│       └── PolyChronos-Omega.md    # The main system prompt (Set this in Cursor)
├── context/
│   └── personas/                   # AI persona definitions (e.g., ProjectManager.md)
├── docs/
│   ├── living/                     # Core planning templates (PRD, Architecture, etc.)
│   └── archives/                   # For historical versions of documents
└── .cursorrules                    # Project-wide quality gates and AI behavior rules
