# GEMINI.md

## Project Overview

The **GL.iNet Toolbox** is a central hub and documentation repository for a collection of tools and scripts designed for GL.iNet routers. Maintained by [@Admon](https://github.com/Admonstrator), a GL.iNet Forum Moderator, it serves as an index for various specialized projects such as Tailscale updaters, AdGuard Home updaters, and ACME certificate managers.

The repository itself does not contain the source code for these tools; instead, it provides a unified landing page with descriptions, compatibility information, and live statistics (stars, forks, latest releases) fetched from the individual tool repositories.

## Directory Overview

This is a **Non-Code Project (Documentation/Hub Repository)**. Its primary function is to provide a user-friendly entry point to the GL.iNet community tools ecosystem.

### Key Files

- **`README.md`**: The main index page. It is a generated file and should not be edited directly.
- **`README.template.md`**: The source template for `README.md`. It contains placeholders (e.g., `{{TAILSCALE_STARS}}`) that are replaced with live data by a GitHub Action.
- **`.github/workflows/update-badges.yml`**: A GitHub Action that runs weekly (or manually) to fetch statistics from the various tool repositories via the GitHub API and regenerate the `README.md`.
- **`images/`**: Contains visual assets like the GL.iNet Robben logo used in the documentation.

## Usage

This repository is intended to be used as a directory:

1.  **Discovery**: Browse the `README.md` to find the tool that matches your needs (e.g., updating Tailscale or AdGuard Home).
2.  **Navigation**: Follow the links to the specific repository for the tool you want to use.
3.  **Community**: Use the provided links to the GL.iNet Forum or Discord for support and discussion.

## Maintenance

The content of `README.md` is automatically maintained:

- **Automatic Updates**: A GitHub Action (`update-badges.yml`) runs every Sunday at midnight to refresh repository statistics.
- **Manual Updates**: The update process can be triggered manually via the "Actions" tab in GitHub using the `workflow_dispatch` event.
- **Templates**: Any permanent changes to the layout or text of the main index should be made in `README.template.md`.
