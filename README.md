# Python Package Manager

[![Visual Studio Marketplace Version](https://img.shields.io/visual-studio-marketplace/v/AkeemMcKenzie.python-package-manager-pro?style=flat-square&logo=visual-studio-code)](https://marketplace.visualstudio.com/items?itemName=AkeemMcKenzie.python-package-manager-pro)
[![Visual Studio Marketplace Installs](https://img.shields.io/visual-studio-marketplace/i/AkeemMcKenzie.python-package-manager-pro?style=flat-square)](https://marketplace.visualstudio.com/items?itemName=AkeemMcKenzie.python-package-manager-pro)
[![Visual Studio Marketplace Downloads](https://img.shields.io/visual-studio-marketplace/d/AkeemMcKenzie.python-package-manager-pro?style=flat-square)](https://marketplace.visualstudio.com/items?itemName=AkeemMcKenzie.python-package-manager-pro)
[![License](https://img.shields.io/badge/license-Proprietary-blue?style=flat-square)](LICENSE)
[![VS Code](https://img.shields.io/badge/VS%20Code-1.90.0+-blue?style=flat-square&logo=visual-studio-code)](https://code.visualstudio.com/)

This extension helps you identify and remove unused Python packages in your projects.

## Features

- **Identify Unused Packages**: Scan your project to find Python packages that are not used in your codebase.
- **Remove Unused Packages**: Easily remove unused Python packages directly from VS Code.
- **Generate Requirements File**: Create a `requirements.txt` file with all currently installed packages.

### Identify Unused Packages

Use the command `Python Package Manager: Identify Unused Python Packages` to scan your project and list unused packages.

![Identify Unused Packages](images/identify-unused-packages.gif)

### Remove Unused Packages

Use the command `Python Package Manager: Remove Unused Python Packages` to uninstall unused packages directly from your virtual environment.

![Remove Unused Packages](images/remove-unused-packages.gif)

### Generate Requirements File

Use the command `Python Package Manager: Generate requirements.txt` to create a `requirements.txt` file with all currently installed packages.

![Generate Requirements File](images/generate-requirements.gif)

## Requirements

- A virtual environment in your project (`venv`, `env`, `.venv`, `.env`).
- Python and pip installed in the virtual environment.
- VS Code installed.

## Extension Settings

This extension does not contribute any settings.

## Known Issues

- The extension currently supports virtual environments with common names only (`venv`, `env`, `.venv`, `.env`). If your virtual environment has a different name, the extension may not detect it.
- The extension may not work correctly if there are multiple virtual environments in the project.

## Release Notes

### 1.0.0

- Initial release of Python Package Manager.
- Added feature to identify unused Python packages.
- Added feature to remove unused Python packages.

### 1.0.1

- Added feature to generate a `requirements.txt` file with installed packages.
- Fix bug fixes relating to checking dependency packages for installed packages.
- Enhanced functionality to remove packages from requirements.txt if they are no longer present.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under a Proprietary License - see the [LICENSE](LICENSE) file for details.

---

**Enjoy managing your Python packages!** 🐍📦