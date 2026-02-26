# Deploy svg2gcode Web App to GitHub Pages

## Analysis
The project already has a GitHub Actions workflow (`.github/workflows/web-deploy.yml`) that automatically deploys to GitHub Pages. It's the simplest solution since:
- Already configured in the repository
- Builds and deploys automatically on push to main branch
- Uses Trunk to build the WASM app (same as your local setup)
- No additional services or accounts needed

## Plan

- [ ] todo-1: Enable GitHub Pages in repository settings
- [ ] todo-2: Push the code to GitHub (initialize git, commit, and push)
- [ ] todo-3: Verify the GitHub Actions workflow runs successfully
- [ ] todo-4: Test the deployed site at the GitHub Pages URL

## Notes
- The workflow triggers when changes are pushed to the main branch
- The site will be available at: `https://<your-github-username>.github.io/svg2gcode-main/`
- The workflow includes `submodules: 'true'` which handles the Spectre CSS submodule
- Build uses `--public-url svg2gcode` for proper asset paths
