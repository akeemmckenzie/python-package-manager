# Python Package Manager

A VS Code extension that helps you identify and remove unused Python packages in your projects, streamlining dependency management and keeping your virtual environments clean.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Configuration](#configuration)
- [Requirements](#requirements)
- [Known Issues](#known-issues)
- [Contributing](#contributing)
- [Release Notes](#release-notes)
- [License](#license)

## Installation

Install the extension from the VS Code Marketplace:

```bash
# Install via VS Code Extensions view
# Search for "Python Package Manager" and click Install

# Or install via command line
code --install-extension python-package-manager
```

Alternatively, you can install from source:

```bash
git clone <repository-url>
cd python-package-manager
npm install
npm run compile
```

## Usage

This extension provides several commands accessible through the VS Code Command Palette (`Ctrl+Shift+P` or `Cmd+Shift+P`):

### Basic Usage Examples

```python
# The extension works with your existing Python projects
# No additional Python imports required - it's a VS Code extension

# Example project structure:
# my-project/
# ├── venv/
# ├── src/
# │   └── main.py
# ├── requirements.txt
# └── ...
```

### Available Commands

1. **Identify Unused Packages**: `Python Package Manager: Identify Unused Python Packages`
2. **Remove Unused Packages**: `Python Package Manager: Remove Unused Python Packages`
3. **Generate Requirements File**: `Python Package Manager: Generate requirements.txt`

## Features

- **Identify Unused Packages**: Scan your project to find Python packages that are not used in your codebase.
- **Remove Unused Packages**: Easily remove unused Python packages directly from VS Code.
- **Generate Requirements File**: Create a `requirements.txt` file with all currently installed packages.

### Identify Unused Packages

Use the command `Python Package Manager: Identify Unused Python Packages` to scan your project and list unused packages.

### Remove Unused Packages

Use the command `Python Package Manager: Remove Unused Python Packages` to uninstall unused packages directly from your virtual environment.

### Generate Requirements File

Use the command `Python Package Manager: Generate requirements.txt` to create a `requirements.txt` file with all currently installed packages.

## Configuration

This extension does not contribute any VS Code settings at this time. The extension automatically detects virtual environments with common names.

## Requirements

- A virtual environment in your project (`venv`, `env`, `.venv`, `.env`)
- Python and pip installed in the virtual environment
- VS Code installed

## Known Issues

- The extension currently supports virtual environments with common names only (`venv`, `env`, `.venv`, `.env`). If your virtual environment has a different name, the extension may not detect it.
- The extension may not work correctly if there are multiple virtual environments in the project.

## Contributing

We welcome contributions to the Python Package Manager extension! Here's how you can help:

### Getting Started

1. Fork the repository
2. Clone your fork locally
3. Install dependencies: `npm install`
4. Make your changes
5. Test your changes thoroughly
6. Submit a pull request

### Development Guidelines

- Follow the existing code style and conventions
- Add tests for new features
- Update documentation as needed
- Ensure all tests pass before submitting

### Reporting Issues

Please report bugs and feature requests through the GitHub Issues page.

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

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Enjoy using Python Package Manager!** 🐍📦