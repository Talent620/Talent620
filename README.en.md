<p align="center">
  <img src="https://raw.githubusercontent.com/Talent620/Talent620/main/assets/portfolio-banner.svg" alt="Artur Józefczak — AI applications, automation, desktop and web" width="100%" />
</p>

[Polski](README.md) · **English**

# Hi, I'm Artur

I develop applications that connect AI with everyday work: documents, communication and product photography. My projects cover interfaces, service integrations, testing and application packaging.

## Selected projects

| Project | What it addresses | Explore |
| :--- | :--- | :--- |
| **JARVIS** | A voice and text assistant combining multiple AI providers, tools and productivity features. | [Source](https://github.com/Talent620/Jarvis) · [Technical overview](projects/jarvis.md) |
| **IMPULS · MARTA** | Document processing and grant documentation assistance with human review of proposed content. | [Public project](https://github.com/Talent620/IMPULS_MARTA_INSTALLER) · [Overview](projects/marta.md) |
| **Sterownik Studio** | AI-assisted product photo editing, source/result comparison and quality checks before export. | [Windows release](https://github.com/Talent620/Sterownik-Studio/releases/tag/v1.9.4) · [Overview](projects/sterownik-studio.md) |

### JARVIS / application integration

The public repository includes a React/TypeScript client, provider adapters, a Cloudflare Worker backend, and desktop/mobile packaging configurations. Areas worth reviewing include provider fallback, tool permissions and the distinction between simulated and confirmed actions.

**React · TypeScript · Vite · Electron · Capacitor · Cloudflare Workers · Vitest**

[Action outcome tests](https://github.com/Talent620/Jarvis/blob/main/tests/actionOutcome.test.ts) · [CI configuration](https://github.com/Talent620/Jarvis/blob/main/.github/workflows/test.yml) · [Architecture](https://github.com/Talent620/Jarvis/blob/main/ARCHITECTURE.md)

### IMPULS · MARTA / document workflow

The workflow moves from source documents through proposed content and human review to files for further checking. The [RC8 test release](https://github.com/Talent620/IMPULS_MARTA_INSTALLER/releases/tag/test-v5.0.0-rc.8) includes an installer, instructions and a report distinguishing controlled tests from the unverified full live-AI workflow. The application does not sign or submit grant applications. The public repository distributes releases; source code is maintained separately.

### Sterownik Studio / image workflow

A Windows application for AI-assisted photo editing with review against the original. Its documented checks cover product identifiers and visible features; uncertain results are blocked from automatic export. The [1.9.4 release](https://github.com/Talent620/Sterownik-Studio/releases/tag/v1.9.4) provides an installer, instructions, checksums and the scope of release verification. Public release materials are separate from the source repository.

## Technologies in these projects

- **Interfaces:** React, TypeScript, Vite, Tailwind CSS.
- **Applications:** Electron, Capacitor, Windows and Linux packaging.
- **Integrations:** AI provider APIs, Cloudflare Workers, agent tools and voice features.
- **Verification:** Vitest, GitHub Actions, type checking, builds and secret scanning.

## Working approach

I use AI coding tools in project development. This portfolio links to implementation and release evidence so reviewers can assess the work directly. Project maturity varies; limitations and verification scope are recorded in the respective documentation.

For a technical conversation, start with [JARVIS: code, tests and a repository map](projects/jarvis.md). Project overviews are currently in Polish; the source code and test files are available through the linked repositories.
