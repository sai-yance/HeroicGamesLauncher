# Custom Windows icon build

This fork includes a manually triggered GitHub Actions workflow at `.github/workflows/custom-windows-installer.yml`.

1. Open the repository's **Actions** tab.
2. Select **Build Windows installer (custom icon)**.
3. Choose **Run workflow** on the `main` branch.
4. Wait for the run to finish successfully.
5. Open the run summary and download the `Heroic-Custom-Icon-Windows-Installer` artifact. Extract the downloaded ZIP and run the setup EXE.

The workflow builds on a GitHub-hosted Windows runner. No local Git, Node.js, pnpm, or development environment is required. The output is an unsigned custom build, not an official Heroic release. The workflow has not yet been run to verify the result.
