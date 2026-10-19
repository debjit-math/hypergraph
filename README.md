# Hypergraph Computation Tools

A static, GitHub Pages-ready collection of independent browser tools.

## Included tools

| Folder | Tool | Notes |
|---|---|---|
| `tools/hypergraph-studio/` | Hypergraph Studio | Edge labels and edge-map output use 1-based edge indexing (`H1`, `H2`, …). Vertex IDs in the input remain 0-based, as required by the original tool. |
| `tools/hypergraph-isomorphism-spectral-analyzer/` | Hypergraph Isomorphism & Spectral Analyzer | Original tool and its README retained. |
| `tools/sum-of-random-variables/` | PMF & Entropy Visualizer | Original tool. |
| `tools/hypergraph-edge-orbits/` | Hypergraph Edge Orbits | Previously unpublished HTML tool; includes a code-analysis README. |

## Run locally

Open `index.html` in a browser. The tools are static HTML and JavaScript. Some tools load libraries from public CDNs, so those features need an internet connection.

## Publish on GitHub Pages

1. Extract this ZIP.
2. Push the contents of this folder to the root of a GitHub repository (the `index.html` should be at repository root).
3. In repository **Settings → Pages**, choose the appropriate branch and root (`/`) as the publishing source.
4. Open the published site URL.

## Add another tool

1. Create a new folder under `tools/`, for example `tools/new-tool/`.
2. Put its entry page at `tools/new-tool/index.html`. Keep supporting files (CSS, JS, images) inside that folder or its subfolders and preserve relative paths.
3. Add a new `<article class="card">…</article>` inside the `<section class="grid">` in the root `index.html`, linking to `tools/new-tool/index.html`.
4. Add a row to the tools table above if you want the documentation to stay up to date.

Use lowercase, hyphen-separated folder names. Avoid duplicate folder names and keep each tool self-contained to prevent file collisions.
