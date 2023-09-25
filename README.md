# Husky pre-commit hooks

[![GitHub license](https://img.shields.io/github/license/fblanc92/husky-precommit-hooks)](LICENSE)

Essential Husky pre-commit hooks for linting, type-checking, testing, file-size monitoring, and code formatting. Simplify and standardize your commit checks with this plug-and-play toolkit.


## Table of Contents

- [Installation](#installation)
- [Features](#features)
- [Usage](#usage)
- [Contribute](#contribute)
- [License](#license)

## Installation

### Prerequisites:
- [Git](https://git-scm.com/)
- [Husky](https://typicode.github.io/husky/#/)


Follow these steps to set up the Commit-Ready Hooks:

1. **Install Husky in your project (if you haven't already):**
   ```bash
   npm install husky --save-dev
   ```
2. Clone this repository or download the hooks you want.
    ```bash
    git clone https://github.com/fblanc92/husky-precommit-hooks.git
    ```

3. Move the hooks into the directory specified by your Husky configuration, typically `.husky/`.
4. Update your `package.json` with the tools in your project, e.g.:
    ```json
    "scripts": {
        "lint": "next lint",
        "format": "prettier --write .",
        "type-check": "tsc --noEmit",
        "test": "jest"
    }
    ```
5. Edit the hooks as necessary to match your development environment and needs.


## Features

- **Linting**: Checks your code for linting issues using ESLint or TSLint.
- **Type-Checking**: Ensures TypeScript types are correct.
- **File-Size Monitoring**: Prevents committing files that are larger than a certain size.
- **Code Formatting**: Formats your staged files using tools like Prettier.
- **Testing**: Runs your tests before committing.

## Usage

Once installed, these hooks will automatically run when committing to your repository, ensuring that your codebase maintains a high quality standard.

To bypass the checks for a particular commit, use the `--no-verify` flag when committing, e.g.:
```bash
git commit -m "Commit message" --no-verify
```
## Contribute
Contributions are always welcome! Check the [CONTRIBUTING.md](CONTRIBUTING.md) for more information.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE) for details.