# Python Package Manager

A VS Code extension that helps you identify and remove unused Python packages in your projects, streamlining dependency management and keeping your virtual environments clean.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
  - [Identify Unused Packages](#identify-unused-packages)
  - [Remove Unused Packages](#remove-unused-packages)
  - [Generate Requirements File](#generate-requirements-file)
- [Configuration](#configuration)
- [Features](#features)
- [Known Issues](#known-issues)
- [Release Notes](#release-notes)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Open VS Code
2. Go to the Extensions view (Ctrl+Shift+X)
3. Search for "Python Package Manager"
4. Click Install

Alternatively, you can install from the VS Code Marketplace or download the VSIX file directly.

## Usage

This extension provides three main commands accessible through the VS Code Command Palette (Ctrl+Shift+P):

### Identify Unused Packages

Scan your project to find Python packages that are not used in your codebase.

```
Python Package Manager: Identify Unused Python Packages
```

This command will:
- Analyze your Python files for import statements
- Compare against installed packages in your virtual environment
- Display a list of unused packages

![Identify Unused Packages]

### Remove Unused Packages

Easily remove unused Python packages directly from VS Code.

```
Python Package Manager: Remove Unused Python Packages
```

This command will:
- Identify unused packages
- Prompt for confirmation before removal
- Uninstall packages from your virtual environment
- Update requirements.txt if packages are removed

![Remove Unused Packages]

### Generate Requirements File

Create a `requirements.txt` file with all currently installed packages.

```
Python Package Manager: Generate requirements.txt
```

This command will:
- Scan your virtual environment for installed packages
- Generate a requirements.txt file with package versions
- Save the file to your project root

![Generate Requirements File]

## Configuration

### Requirements

- **Virtual Environment**: A virtual environment in your project with one of these common names:
  - `venv`
  - `env`
  - `.venv`
  - `.env`
- **Python**: Python installed in the virtual environment
- **pip**: pip package manager available in the virtual environment
- **VS Code**: Visual Studio Code installed

### Extension Settings

This extension does not contribute any configurable settings at this time.

## Features

- **Identify Unused Packages**: Scan your project to find Python packages that are not used in your codebase
- **Remove Unused Packages**: Easily remove unused Python packages directly from VS Code
- **Generate Requirements File**: Create a `requirements.txt` file with all currently installed packages
- **Smart Dependency Detection**: Enhanced functionality to handle dependency packages correctly
- **Requirements.txt Integration**: Automatically updates requirements.txt when packages are removed

## Known Issues

- The extension currently supports virtual environments with common names only (`venv`, `env`, `.venv`, `.env`). If your virtual environment has a different name, the extension may not detect it.
- The extension may not work correctly if there are multiple virtual environments in the project.
- Complex dependency relationships may not be fully resolved in some edge cases.

## Release Notes

### 1.0.1
- Added feature to generate a `requirements.txt` file with installed packages
- Fixed bug fixes relating to checking dependency packages for installed packages
- Enhanced functionality to remove packages from requirements.txt if they are no longer present

### 1.0.0
- Initial release of Python Package Manager
- Added feature to identify unused Python packages
- Added feature to remove unused Python packages

## Contributing

We welcome contributions to the Python Package Manager extension! Here's how you can help:

### Getting Started
1. Fork the repository
2. Clone your fork locally
3. Install dependencies: `npm install`
4. Make your changes
5. Test your changes thoroughly
6. Submit a pull request

### Guidelines
- Follow the existing code style and conventions
- Add tests for new features
- Update documentation as needed
- Ensure all tests pass before submitting

### Reporting Issues
Please report bugs and feature requests through the GitHub Issues page.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

For more information, visit the [GitHub repository](https://github.com/your-username/python-package-manager) or check out the [VS Code Marketplace page](https://marketplace.visualstudio.com/items?itemName=your-publisher.python-package-manager).