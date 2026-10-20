# Custom Windows icon build

This fork can build a Windows installer entirely in GitHub Actions. No local development tools are needed.

## One-time icon upload

Upload your generated `win_icon_high_quality.ico` through GitHub's web UI to this exact repository path:

`public/custom_win_icon.ico`

Use the repository's **Add file → Upload files** action and commit the uploaded file to `main`. The custom workflow copies that file into `build/win_icon.ico` after the application build, just before packaging.

## Build the installer

1. Open the **Actions** tab.
2. Select **Build Windows installer (custom icon)**.
3. Click **Run workflow** and choose `main`.
4. Wait for the workflow to finish successfully.
5. Open the run summary and download the `Heroic-Custom-Icon-Windows-Installer` artifact.
6. Extract the downloaded ZIP and run the setup EXE.

The build runs on a GitHub-hosted Windows runner. The resulting custom build is unsigned and is not an official Heroic release. The workflow has not yet been run to verify its output.
