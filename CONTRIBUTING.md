# Contributing to QuarryAI

This repository is primarily a public website and documentation project. Before contributing, check the current repository state and confirm that the owner wants changes to be accepted.

## Project scope

The repository currently contains:

- the public QuarryAI landing page
- deployment configuration for GitHub Pages
- repository and documentation files

This is not a full Java/Maven/Paper plugin project in the current snapshot, so contributions should focus on accuracy, clarity, documentation quality, and project presentation rather than code changes that imply unsupported platform features.

## Prerequisites

To contribute effectively, you should have:

- a GitHub account
- a local git checkout
- a text editor or IDE
- a browser for previewing the static site
- basic Markdown and HTML knowledge

## Local setup

Clone the repository and open it in your editor:

```bash
git clone https://github.com/ItzJatinOG/Quarry.git
cd Quarry
```

To preview the static page locally:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000` in a browser.

## Documentation expectations

Keep documentation accurate and repository-faithful. In particular:

- do not claim features that are not supported by the checked-in project files
- do not invent product capabilities or backend architecture
- disclose uncertainty when a fact cannot be verified from the repo
- keep descriptions of QuarryAI precise and consistent with the public website
- prefer clear, helpful writing over SEO-heavy filler

## Pull request guidelines

When submitting changes:

- keep the scope focused
- explain the reason for the change clearly
- update docs where the product description or behavior changes
- ensure links are valid and relative where appropriate
- avoid unrelated formatting churn or broad rewrites

## Security and privacy expectations

Do not include:

- API keys
- tokens
- credentials
- private endpoints
- personal user data
- secret configuration values

If you are documenting security practices or examples, keep them generic and safe.

## Reporting issues

If you encounter a problem with the documentation or repository content:

1. review whether the issue is already documented
2. open a clear issue with steps to reproduce
3. explain the expected behavior and the actual behavior
4. include relevant context without exposing private data

Because this repository does not currently include a designated security email or policy channel, any private security report should be handled by the repository owner through a secure, explicit reporting mechanism when one is configured.

## Summary

Contributions are most helpful when they improve accuracy, clarity, and maintainability. The repository is best served by honest documentation that reflects the current project state and the public QuarryAI website without overstating unsupported functionality.
