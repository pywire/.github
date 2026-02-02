# pywire

### The Live Conduit for Python and the Web.

**pywire v0.1.0 is now available!** 🚀

**pywire** is a Python HTML-over-the-wire framework that combines server-side logic with reactive HTML templates in single `.wire` files. It bridges the gap between your backend and frontend with a persistent, real-time connection.

---

### Core Philosophy

* **⚡️ Instant Reactivity:** State changes on the server are reflected in the browser instantly via WebTransport/WebSocket.
* **🧬 Single-File Components:** Write Python logic and HTML structure in one `.wire` file.
* **🔋 Zero Boilerplate:** No API endpoints, no serializers, no complex JavaScript build steps.

### The Ecosystem

| Repository | Description |
| :--- | :--- |
| [**pywire**](https://github.com/pywire/pywire) | The core framework, CLI, and runtime. |
| [**create-pywire-app**](https://github.com/pywire/create-pywire-app) | Official project bootstrapping tool. |
| [**vscode-pywire**](https://github.com/pywire/vscode-pywire) | Syntax highlighting, snippets, and LSP integration for VS Code. |
| [**pywire-language-server**](https://github.com/pywire/pywire-language-server) | Language Server Protocol implementation for `.wire` files. |
| [**examples**](https://github.com/pywire/examples) | Reference implementations and community examples. |

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

### Community & Support

* 💬 **Discord:** [Join the Community](https://pywire.dev/discord) - Get help and discuss ideas.
* 🐞 **Bugs:** Please file issues in the [pywire/pywire](https://github.com/pywire/pywire/issues) repository.
* 📖 **Docs:** Read the full documentation at [pywire.dev](https://pywire.dev).

---

<div align="center">
  <sub>Built with the speed of Python and the power of the Web.</sub>
</div>
