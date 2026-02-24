# Python Package Manager

A VS Code extension that helps you identify and remove unused Python packages in your projects, keeping your development environment clean and efficient.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Features](#features)
- [Known Issues](#known-issues)
- [Contributing](#contributing)
- [Release Notes](#release-notes)
- [License](#license)

## Installation

This extension can be installed directly from the VS Code marketplace:

1. Open VS Code
2. Go to Extensions (Ctrl+Shift+X)
3. Search for "Python Package Manager"
4. Click Install

Alternatively, you can install it via the command line:

```bash
code --install-extension python-package-manager
```

## Usage

The extension provides three main commands accessible through the VS Code Command Palette (Ctrl+Shift+P):

### Identify Unused Packages

```
Python Package Manager: Identify Unused Python Packages
```

This command scans your project to find Python packages that are not used in your codebase and displays them in a list.

### Remove Unused Packages

```
Python Package Manager: Remove Unused Python Packages
```

This command allows you to uninstall unused packages directly from your virtual environment, helping keep your project dependencies clean.

### Generate Requirements File

```
Python Package Manager: Generate requirements.txt
```

This command creates a `requirements.txt` file with all currently installed packages in your virtual environment.

## Configuration

### Requirements

- A virtual environment in your project with one of the following names:
  - `venv`
  - `env`
  - `.venv`
  - `.env`
- Python and pip installed in the virtual environment
- VS Code installed

### Extension Settings

This extension does not contribute any configurable settings at this time.

## Features

- **Identify Unused Packages**: Scan your project to find Python packages that are not used in your codebase
- **Remove Unused Packages**: Easily remove unused Python packages directly from VS Code
- **Generate Requirements File**: Create a `requirements.txt` file with all currently installed packages
- **Virtual Environment Detection**: Automatically detects common virtual environment configurations
- **Requirements.txt Management**: Enhanced functionality to remove packages from requirements.txt if they are no longer present

## Known Issues

- The extension currently supports virtual environments with common names only (`venv`, `env`, `.venv`, `.env`). If your virtual environment has a different name, the extension may not detect it.
- The extension may not work correctly if there are multiple virtual environments in the project.

## Contributing

We welcome contributions to improve Python Package Manager! Here's how you can help:

### Getting Started

1. Fork the repository
2. Clone your fork locally
3. Create a new branch for your feature or bug fix
4. Make your changes
5. Test your changes thoroughly
6. Submit a pull request

### Guidelines

- Follow the existing code style and conventions
- Add tests for new features
- Update documentation as needed
- Ensure all tests pass before submitting

### Reporting Issues

If you encounter any bugs or have feature requests, please open an issue on the project repository with:

- A clear description of the problem or feature request
- Steps to reproduce (for bugs)
- Your environment details (VS Code version, Python version, OS)

## Release Notes

### 1.0.1

- Added feature to generate a `requirements.txt` file with installed packages
- Fixed bug fixes relating to checking dependency packages for installed packages
- Enhanced functionality to remove packages from requirements.txt if they are no longer present

### 1.0.0

- Initial release of Python Package Manager
- Added feature to identify unused Python packages
- Added feature to remove unused Python packages

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

**Enjoy using Python Package Manager!** 🐍📦