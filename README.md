# Python Package Manager

A VS Code extension that helps you identify and remove unused Python packages in your projects, streamline dependency management, and maintain clean requirements files.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
  - [Identify Unused Packages](#identify-unused-packages)
  - [Remove Unused Packages](#remove-unused-packages)
  - [Generate Requirements File](#generate-requirements-file)
- [Configuration](#configuration)
  - [Requirements](#requirements)
  - [Extension Settings](#extension-settings)
- [Known Issues](#known-issues)
- [Contributing](#contributing)
- [License](#license)
- [Changelog](#changelog)

## Installation

Install the Python Package Manager extension from the VS Code marketplace:

1. Open VS Code
2. Go to Extensions (Ctrl+Shift+X)
3. Search for "Python Package Manager"
4. Click Install

Alternatively, you can install it via command line:

```bash
code --install-extension python-package-manager
```

## Usage

This extension provides three main commands accessible through the VS Code Command Palette (Ctrl+Shift+P):

### Identify Unused Packages

Scan your project to find Python packages that are not used in your codebase.

**Command:** `Python Package Manager: Identify Unused Python Packages`

```python
# The extension will analyze your Python files and compare against installed packages
# to identify unused dependencies in your virtual environment
```

![Identify Unused Packages]

### Remove Unused Packages

Easily remove unused Python packages directly from VS Code.

**Command:** `Python Package Manager: Remove Unused Python Packages`

```python
# This command will:
# 1. Identify unused packages
# 2. Prompt you to confirm removal
# 3. Uninstall packages from your virtual environment
# 4. Update requirements.txt if present
```

![Remove Unused Packages]

### Generate Requirements File

Create a `requirements.txt` file with all currently installed packages.

**Command:** `Python Package Manager: Generate requirements.txt`

```python
# Generates a requirements.txt file in your project root with format:
# package-name==version
# another-package==version
```

![Generate Requirements File]

## Configuration

### Requirements

- A virtual environment in your project (`venv`, `env`, `.venv`, `.env`)
- Python and pip installed in the virtual environment
- VS Code installed

### Extension Settings

This extension does not contribute any VS Code settings at this time. All functionality is accessed through command palette commands.

## Known Issues

- The extension currently supports virtual environments with common names only (`venv`, `env`, `.venv`, `.env`). If your virtual environment has a different name, the extension may not detect it.
- The extension may not work correctly if there are multiple virtual environments in the project.
- Dependency analysis may not catch dynamically imported packages or packages imported in non-standard ways.

## Contributing

We welcome contributions to the Python Package Manager extension! Here's how you can help:

### Getting Started

1. Fork the repository
2. Clone your fork locally
3. Install dependencies
4. Make your changes
5. Test your changes
6. Submit a pull request

### Development Setup

```bash
# Clone the repository
git clone https://github.com/your-username/python-package-manager.git
cd python-package-manager

# Install dependencies
npm install

# Open in VS Code
code .
```

### Reporting Issues

Please report bugs and feature requests through the GitHub issue tracker. Include:

- VS Code version
- Python version
- Virtual environment setup
- Steps to reproduce the issue

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Changelog

### 1.0.1

- Added feature to generate a `requirements.txt` file with installed packages
- Fixed bug fixes relating to checking dependency packages for installed packages
- Enhanced functionality to remove packages from requirements.txt if they are no longer present

### 1.0.0

- Initial release of Python Package Manager
- Added feature to identify unused Python packages
- Added feature to remove unused Python packages