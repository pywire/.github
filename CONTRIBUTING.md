# Contributing to pywire

Thank you for your interest in contributing to pywire! 🧡

pywire is an open-source project, and we welcome contributions of all forms, whether it's reporting bugs, improving documentation, or writing code.

We strive to be an inclusive and welcoming community. Please be professional and respectful in all interactions.

## 🚀 Ways to contribute

* **Reporting Bugs:** If you find a bug, please create an issue in the relevant repository within the [pywire organization](https://github.com/pywire).
* **Suggesting Features:** We love hearing new ideas! Please open a discussion or issue to discuss the design before writing code.
* **Documentation:** Improvements to docs are just as important as code.
* **Code:** Help us maintain and improve the pywire framework.

## 🛠 Development

pywire is a polyrepo organization. These instructions generally apply to the `pywire` core repository and related repositories in the workspace.

### Prerequisites

* **Python:** You need Python 3.11 through 3.14.
* **uv:** We use [uv](https://github.com/astral-sh/uv) for dependency management.
* **pnpm:** You may need [pnpm](https://github.com/pnpm/pnpm) (v9+) for working with the pywire client and websites.
* **Git:** Version control.

### Setup

1.  **Fork** the repository you want to work on (e.g., `pywire/pywire`) to your own GitHub account.
2.  **Clone** your fork to your local machine:

    ```bash
    git clone https://github.com/your-username/pywire.git
    cd pywire
    ```

3.  **Set up your environment**. We use `uv` to manage the workspace and dependencies:

    ```bash
    ./scripts/install
    ```

4.  **Initialize the project**. Ensure you have the necessary tools installed (like `pnpm` for documentation and client work).

    We provide several helper scripts in the `scripts/` directory to make development easier. Here are the most common ones (available in `pywire` and most sub-repositories):

    *   `scripts/docs`: Runs the documentation development server (requires `pnpm`).
    *   `scripts/build`: Builds the client and documentation (requires `pnpm`).
    *   `scripts/check`: Runs the full suite of checks (formatting, linting, type checking, and tests).
    *   `scripts/lint`: Automatically formats code and fixes linting errors.
    *   `scripts/test`: Runs the test suite.

### Code Style

We enforce strict code style to keep the codebase clean and readable. We use [Ruff](https://github.com/astral-sh/ruff) for both formatting and linting, and [mypy](https://mypy-lang.org/) for static type checking.

*   **Format/Fix:** Run `./scripts/lint` to automatically format and fix linting errors.
*   **Verify:** Run `./scripts/check` to verify that everything (formatting, types, tests) is correct.

### Running Tests

We use `pytest` for testing. Please ensure all tests pass before submitting a Pull Request.

```bash
./scripts/test
```

If you are adding a new feature, please add a corresponding test case in the `tests/` directory.

## 📝 Documentation

Documentation is built using Starlight/Astro. If you are contributing to the documentation (usually in the `docs` folder or a separate `pywire-docs` repo):

1.  Navigate to the docs directory (or use `scripts/docs` from the root of `pywire`).
2.  Install dependencies via `pnpm`.
3.  Run the development server to preview changes.

## ⚖️ License & DCO

pywire is licensed under the **Apache 2.0 License**.

To ensure that you have the right to contribute your code, we require all changes to be "Signed-off". This certifies that you wrote the code or have the right to contribute it (Developer Certificate of Origin).

You can sign off your commits by adding the `-s` flag:

```bash
git commit -s -m "feat: add new signal handling to server"
```

##  Pull Requests

1.  **Create a branch** for your changes:
    ```bash
    git checkout -b my-new-feature
    ```
2.  **Make your changes**. We prefer uses of [Conventional Commits](https://www.conventionalcommits.org/) for commit messages (e.g., `feat: add new signal handling to server`).
3.  **Commit them** (remember to sign-off!).
4.  **Push** your branch to your fork.
5.  **Open a Pull Request** against the `main` branch of the upstream repository.

### Checklist for a great PR:
* [ ] The code follows the code style (run `./scripts/lint`).
* [ ] You have added tests for new features.
* [ ] All tests pass (run `./scripts/check`).
* [ ] You have updated the documentation (if applicable).
* [ ] You have signed off your commits.

Thank you for contributing!