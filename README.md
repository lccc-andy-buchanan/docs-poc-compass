# Compass — documentation workflow fixture

This fictional public project owns only its Markdown documentation and a small Docker preview configuration. No renderer, Node dependencies or deployment machinery live here.

```sh
docker compose up docs-preview
```

Open http://localhost:4321. Your local `docs/` replaces Compass in the complete three-project site and live-reloads as you edit. The renderer fetches the other public projects automatically and caches them in a named volume. Only Docker is required; no registry or GitHub login is needed to preview.

Create a branch (or fork), edit the docs, preview locally, and open a PR to this repository. Deployment is handled separately by the private GitLab control plane.
