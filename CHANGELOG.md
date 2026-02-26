# Change Log

All notable changes to the "python-package-manager" extension will be documented in this file.

Check [Keep a Changelog](http://keepachangelog.com/) for recommendations on how to structure this file.

## [1.0.1] - 2024-01-15

### Added
- Feature to generate a `requirements.txt` file with installed packages
- Enhanced functionality to remove packages from requirements.txt if they are no longer present

### Fixed
- Bug fixes relating to checking dependency packages for installed packages

## [1.0.0] - 2024-01-01

### Added
- Initial release of Python Package Manager
- Feature to identify unused Python packages in your project
- Feature to remove unused Python packages directly from VS Code
- Support for common virtual environment names (`venv`, `env`, `.venv`, `.env`)
- Integration with VS Code command palette

### Requirements
- VS Code 1.90.0 or higher
- Python and pip installed in virtual environment
- Virtual environment in project directory