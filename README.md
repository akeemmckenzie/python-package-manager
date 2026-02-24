# Python Package Manager

A VS Code extension that helps you identify and remove unused Python packages in your projects, streamlining dependency management and keeping your virtual environments clean.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)
- [Release Notes](#release-notes)

## Installation

This extension is available through the VS Code Extension Marketplace. To install:

1. Open VS Code
2. Go to the Extensions view (Ctrl+Shift+X)
3. Search for "Python Package Manager"
4. Click Install

Alternatively, you can install it via the command line:

```bash
code --install-extension python-package-manager
```

## Usage

The Python Package Manager extension provides three main features to help manage your Python dependencies:

### Identify Unused Packages

Scan your project to find Python packages that are not used in your codebase.

**Command**: `Python Package Manager: Identify Unused Python Packages`

1. Open the Command Palette (Ctrl+Shift+P)
2. Type "Python Package Manager: Identify Unused Python Packages"
3. Press Enter to execute
4. View the list of unused packages in the output panel

### Remove Unused Packages

Easily remove unused Python packages directly from your virtual environment.

**Command**: `Python Package Manager: Remove Unused Python Packages`

1. Open the Command Palette (Ctrl+Shift+P)
2. Type "Python Package Manager: Remove Unused Python Packages"
3. Press Enter to execute
4. Confirm the removal of unused packages
5. Packages will be uninstalled from your virtual environment

### Generate Requirements File

Create a `requirements.txt` file with all currently installed packages.

**Command**: `Python Package Manager: Generate requirements.txt`

1. Open the Command Palette (Ctrl+Shift+P)
2. Type "Python Package Manager: Generate requirements.txt"
3. Press Enter to execute
4. A `requirements.txt` file will be created in your project root

## Configuration

### Requirements

- A virtual environment in your project (`venv`, `env`, `.venv`, `.env`)
- Python and pip installed in the virtual environment
- VS Code installed

### Extension Settings

This extension does not contribute any VS Code settings at this time.

### Known Issues

- The extension currently supports virtual environments with common names only (`venv`, `env`, `.venv`, `.env`). If your virtual environment has a different name, the extension may not detect it.
- The extension may not work correctly if there are multiple virtual environments in the project.

## Contributing

We welcome contributions to the Python Package Manager extension! Here's how you can help:

### Getting Started

1. Fork the repository
2. Clone your fork locally
3. Install dependencies
4. Make your changes
5. Test your changes thoroughly
6. Submit a pull request

### Guidelines

- Follow the existing code style and conventions
- Add tests for new features
- Update documentation as needed
- Ensure all tests pass before submitting

### Reporting Issues

If you encounter any bugs or have feature requests, please open an issue on our GitHub repository with:

- A clear description of the problem or feature request
- Steps to reproduce (for bugs)
- Your environment details (VS Code version, Python version, OS)

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Release Notes

### 1.0.1

- Added feature to generate a `requirements.txt` file with installed packages
- Fixed bug fixes relating to checking dependency packages for installed packages
- Enhanced functionality to remove packages from requirements.txt if they are no longer present

### 1.0.0

- Initial release of Python Package Manager
- Added feature to identify unused Python packages
- Added feature to remove unused Python packages