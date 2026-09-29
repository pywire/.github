# pywire

### The Live Conduit for Python

**pywire** is an HTML-over-the-wire web framework for Python. The server renders HTML and streams DOM updates to the browser over WebSocket, so you get an interactive app without writing JavaScript, a JSON API, or client state sync.

Pages and components are `.wire` files: Python, HTML, CSS and optional JS in one file.

```pywire
---
count = wire(0)
---
<button @click={count += 1}>Clicked {count} times</button>
```

<!-- INSTALL_MESSAGE_TEMPLATE_START -->
## Quick start

Use whichever tool you already have. All three launch the same wizard:

```sh
uvx create-pywire-app                              # uv (recommended)
npx create-pywire-app                              # Node.js, installs uv if missing
curl -fsSL https://pywire.dev/install | sh         # neither: installs uv, then the wizard
```

On Windows (PowerShell): `irm https://pywire.dev/install.ps1 | iex`
<!-- INSTALL_MESSAGE_TEMPLATE_END -->

### Where things live

Everything except the marketing site is developed in one monorepo.

| Repository | What it holds |
| :--- | :--- |
| [**pywire/pywire**](https://github.com/pywire/pywire) | Core framework, parser, CLI, auth, language server, VS Code extension, Prettier plugin, tree-sitter grammar, create-pywire-app, docs and examples. Issues go here. |
| [**pywire/pywire.dev**](https://github.com/pywire/pywire.dev) | The [pywire.dev](https://pywire.dev) marketing site and its infrastructure. |

The older standalone repositories (pywire-core, pywire-language-server, vscode-pywire, prettier-plugin-pywire, tree-sitter-pywire, create-pywire-app, examples, pywire-workspace) are no longer updated. Their code now lives in the monorepo.

### Links

* **Docs:** [pywire.dev/docs](https://pywire.dev/docs)
* **Bugs and feature requests:** [pywire/pywire issues](https://github.com/pywire/pywire/issues)
* **Questions and ideas:** [pywire/pywire discussions](https://github.com/pywire/pywire/discussions)
* **Contributing:** see the [contributing guide](https://github.com/pywire/.github/blob/main/CONTRIBUTING.md)

Licensed under Apache-2.0.
