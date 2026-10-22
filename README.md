# QuarryAI — AI Minecraft Paper Plugin Generator

QuarryAI is an AI-powered Minecraft Paper plugin generator that helps server owners and developers turn natural-language plugin ideas into Paper-oriented Java source and compiled plugin workflows. The live product is hosted at [quarryai.dpdns.org](https://quarryai.dpdns.org/).

## Project overview

This repository currently contains the public QuarryAI website and documentation rather than a full Java/Maven/Paper plugin project. Based on the code in this snapshot, the project is primarily a static web landing page and documentation hub for the QuarryAI service.

The visible source includes:

- a static marketing landing page in [index.html](index.html)
- a GitHub Pages deployment workflow in [.github/workflows/static.yml](.github/workflows/static.yml)
- repository documentation in the [docs](docs) folder

The repository does not currently include a package manifest, application server source, or a Java project structure that would support building and testing a Paper plugin locally. That means the most accurate description for this repo is: a website and documentation repository for an AI-powered Paper plugin generator, not a complete plugin source tree.

## What QuarryAI helps with

QuarryAI is intended to help Minecraft server owners and developers move from an idea to a plugin workflow more quickly. The website messaging in this repository suggests a flow where a user describes a plugin in plain language, reviews generated Java code, selects a model, and downloads a compiled plugin file for use on a Paper server.

This is most relevant when someone wants to prototype:

- home or teleport systems
- economy and player shop features
- moderation tools
- spawn protection or admin utilities
- custom server quality-of-life plugins

## Features and verified repository evidence

The following are supported by the current project files:

- a static public website for QuarryAI
- AI-themed plugin-generation messaging for Paper servers
- promotion of multiple model choices, including Gemini and ChatGPT references
- a landing page explaining a workflow from prompt to compiled .jar
- examples, guides, FAQ, and pricing links on the public website
- documentation pages intended to help users learn plugin basics and installation steps

The repository does not contain verified implementation details for:

- a hosted backend service
- a secure API architecture
- a Java plugin source generator codebase
- plugin generation from a private application source that is not included here
- a formal license or contribution policy

## Example use cases

The following are realistic examples based on typical Minecraft server plugin needs and the repository's messaging. They are presented as examples or ideas rather than verified product guarantees:

- Home and teleportation systems
- Player shops and economy features
- Chat moderation and anti-spam tools
- Spawn protection and admin utilities
- Custom commands for server quality-of-life improvements
- Event or mini-game helpers for Paper servers

## Screenshots and demos

This repository does not currently contain dedicated screenshot assets or demo image files. The landing page in [index.html](index.html) includes a browser mockup that describes the app flow, but there are no stored screenshots or media files in the repo snapshot.

## Getting started

This repository is a static site and documentation project. To view or edit it locally:

1. Clone the repository.
2. Open [index.html](index.html) in a browser for a quick local preview.
3. Or serve the folder with a static web server if you want a browser preview that matches GitHub Pages behavior.

Example:

```bash
cd /path/to/Quarry
python3 -m http.server 8000
```

Then open `http://localhost:8000` in a browser.

There is no package.json, lockfile, or build pipeline in the current snapshot. The deployment flow in [.github/workflows/static.yml](.github/workflows/static.yml) uploads the repository as a GitHub Pages static site.

## Documentation links

Official website:

- [QuarryAI](https://quarryai.dpdns.org/)
- [Examples](https://quarryai.dpdns.org/examples)
- [Guides](https://quarryai.dpdns.org/guides)
- [FAQ](https://quarryai.dpdns.org/faq)
- [Pricing](https://quarryai.dpdns.org/pricing)

Repository documentation:

- [docs/README.md](docs/README.md)
- [docs/paper-plugin-guide.md](docs/paper-plugin-guide.md)
- [docs/plugin-installation.md](docs/plugin-installation.md)
- [docs/minecraft-plugin-ideas.md](docs/minecraft-plugin-ideas.md)
- [docs/troubleshooting.md](docs/troubleshooting.md)
- [docs/seo-and-brand.md](docs/seo-and-brand.md)

## Limitations and compatibility

This repository does not provide a verified compatibility matrix for Paper versions, Java versions, or plugin platform support. The site references Paper-friendly workflows, and the repository is oriented around Paper server use, but no explicit Java runtime or Paper version requirement file is included in the checked-in code.

Important limitations to keep in mind:

- This repo is not a complete standalone Paper plugin project.
- No verified build or test command was found for a plugin generator backend.
- No license file is present, so license and reuse terms are not established in this repository snapshot.
- The public website may describe a hosted service that is not fully represented in repository source.

## Security

This repository is a public docs and static-site repo, so the main security expectations are:

- never publish secret API keys, tokens, private endpoints, or credentials
- never share private server data or user content in issues or pull requests
- treat generated plugin code as untrusted until reviewed in a safe testing environment
- avoid running unverified code or downloaded plugins in production servers

## Contributing

The repository does not currently include a clear contribution policy, code of conduct, or license file. Before proposing changes, confirm the project owner’s intent and preferred workflow.

If contributions are enabled in the future, a typical contribution flow would be:

1. review this README and the docs
2. keep edits truthful and repository-accurate
3. avoid claiming unsupported product capabilities
4. open a focused pull request with clear context and examples

See [CONTRIBUTING.md](CONTRIBUTING.md) for the repository’s contribution guidance.

## License

No license file was found in this repository snapshot. Because of that, the project should not be assumed to be open source under a specific license unless the repository owner confirms that clearly.

## Repository metadata recommendations

The following metadata is consistent with the repository content and the public website:

- Product name: QuarryAI
- Official website: https://quarryai.dpdns.org/
- Public description: "QuarryAI is an AI-powered Minecraft Paper plugin generator that helps server owners create custom plugins from natural-language descriptions."

GitHub About and topic settings can be updated through the GitHub UI, but they are not controlled from this repository snapshot.

## Status of this repo

This repository is a documentation and static web presence for QuarryAI. It is useful for onboarding, discovery, and public-facing documentation, but it does not appear to be the complete generator application or a full plugin source project.

That distinction matters: the docs in this repository should describe the available public product accurately without claiming direct access to code or infrastructure that is not present here.

