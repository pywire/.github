# Contributing to pywire

Thanks for your interest in pywire. Bug reports, docs improvements and code are all welcome. Please be respectful in every interaction.

## Ways to contribute

* **Bugs:** open an issue in [pywire/pywire](https://github.com/pywire/pywire/issues). Include a small `.wire` snippet and your pywire version if you can.
* **Features:** open a [discussion](https://github.com/pywire/pywire/discussions) or an issue to talk through the design before writing code.
* **Docs:** improvements are as useful as code. The docs live in `docs/` in the monorepo.
* **Code:** see below.

## Development

pywire is a monorepo. All packages are developed and released from [pywire/pywire](https://github.com/pywire/pywire), and the repo's `AGENTS.md` is the full reference for build, test and conventions. The marketing site is in [pywire/pywire.dev](https://github.com/pywire/pywire.dev).

### Prerequisites

* Python 3.11 to 3.14
* [uv](https://docs.astral.sh/uv/) for Python packages
* [pnpm](https://pnpm.io/) 10 and Node 24 for JS packages, docs and the browser client (use pnpm, not npm)
* A Rust toolchain if you touch the tree-sitter grammar tests
* Git

### Setup

1. Fork [pywire/pywire](https://github.com/pywire/pywire) and clone your fork:

    ```sh
    git clone https://github.com/your-username/pywire.git
    cd pywire
    ```

2. Install everything:

    ```sh
    ./scripts/install
    ```

Useful scripts, from the repo root or any package directory:

* `./scripts/check`: format, lint, type check and tests. Use `./scripts/check --changed` to run only the packages your change affects.
* `./scripts/test`: run the test suites.
* `./scripts/lint`: format code and fix lint errors.

### Code style

Python uses ruff for formatting and linting and ty for type checking. TypeScript uses prettier, eslint and tsc. Run `./scripts/check` before opening a PR. If you add a feature or fix a bug, add a test in the package's `tests/` directory.

## Pull requests

1. Create a branch for your change.
2. Use [Conventional Commits](https://www.conventionalcommits.org/) for commit messages and PR titles, for example `feat(pywire): add signal batching`. Releases are generated from them. Don't put extra parentheses in a PR title beyond the scope, and don't bump versions by hand.
3. Open the PR against `main`. PRs are squash-merged and need one approving review and passing CI.

Checklist:

* [ ] `./scripts/check` passes.
* [ ] New behavior has tests.
* [ ] Docs are updated if needed.

## License

pywire is licensed under Apache-2.0. By contributing, you agree that your contributions are licensed under the same terms.
