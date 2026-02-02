# pywire

### The Live Conduit for Python and the Web.

> **🚧 Migration in Progress**
> 
> **pywire** is currently migrating from its original home at [reecelikesramen/pyhtml](https://github.com/reecelikesramen/pyhtml). 
> We are in the process of moving the core runtime, tooling, and documentation to this new organization. Expect rapid changes and some broken links as we settle into our new `.wire` architecture.

**pywire** is a Python HTML-over-the-wire framework that combines server-side logic with reactive HTML templates in single `.wire` files. It bridges the gap between your backend and frontend with a persistent, real-time connection.

---

### Core Philosophy

* **⚡️ Instant Reactivity:** State changes on the server are reflected in the browser instantly via WebTransport/WebSocket.
* **🧬 Single-File Components:** Write Python logic and HTML structure in one `.wire` file.
* **🔋 Zero Boilerplate:** No API endpoints, no serializers, no complex JavaScript build steps.

### The Ecosystem

| Repository | Description |
| :--- | :--- |
| [**pywire**](https://github.com/pywire/pywire) | The core framework, CLI, and runtime. Start here. |
| [**vscode-pywire**](https://github.com/pywire/vscode-pywire) | Official VS Code extension for syntax highlighting and snippets. |
| [**pywire-language-server**](https://github.com/pywire/pywire-language-server) | The brain behind the tooling. LSP implementation for `.wire` files. |
| [**examples**](https://github.com/pywire/examples) | Real-world examples. |

<!-- INSTALL_MESSAGE_TEMPLATE_START -->
## 🚀 Quick Start

If you already have [uv](https://docs.astral.sh/uv/) installed, you can get started instantly:

```bash
uvx create-pywire-app
```

If you don't have `uv` installed or aren't sure, use our installer script which handles the setup for you:

### macOS / Linux
```bash
curl -fsSL pywire.dev/install | sh
```

### Windows (PowerShell)
```powershell
irm pywire.dev/install.ps1 | iex
```
<!-- INSTALL_MESSAGE_TEMPLATE_END -->

<!--### Community & Support

* 💬 **Discord:** [Join the Community](https://pywire.dev/discord) - Get help and discuss ideas.
* 🐞 **Bugs:** Please file issues in the [pywire/pywire](https://github.com/pywire/pywire/issues) repository.
* 📖 **Docs:** Read the full documentation at [pywire.dev](https://pywire.dev).-->

---

<div align="center">
  <sub>Built with the speed of Python and the power of the Web.</sub>
</div>
