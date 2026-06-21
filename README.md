# Resume — ARSALAN KHAN

This repository stores a single-source resume (resume.md) and an automated workflow to produce resume.pdf on every push to the `main` branch.

How to edit
- Edit resume.md directly on GitHub or clone the repo, edit locally, then push your changes.
- Commits to `main` will trigger the GitHub Action that builds resume.pdf.

How the workflow works
- Uses a pandoc Docker image (pandoc/extra:3.5) with the Eisvogel LaTeX template to convert resume.md -> resume.pdf.
- The action uploads resume.pdf as a build artifact and also pushes the PDF to a `pdf` branch for direct download.

Options you can change
- Use a different pandoc template (Eisvogel is included by default in the workflow).
- Publish resume.pdf via GitHub Pages or attach it to releases — request this and I’ll update the workflow.
