# Copilot Instructions for Python Virtual Environment

## Architecture Overview
This workspace is a Python virtual environment (venv) created with Python 3.13.9, providing isolated package management for Python projects.

- **Major Components**: 
  - `Scripts/`: Contains activation scripts and pip executable
  - `Lib/site-packages/`: Installed packages directory
  - `pyvenv.cfg`: Configuration file specifying Python version and paths

- **Data Flows**: Standard Python execution with isolated dependencies

## Developer Workflows
- **Activation**: Run `Scripts\activate.bat` in PowerShell to activate the environment
- **Package Installation**: Use `pip install <package>` for dependencies
- **Script Execution**: Run `python <script.py>` for Python files
- **Deactivation**: Run `deactivate` to exit the environment

## Conventions and Patterns
- Use pip for all package management
- Avoid installing packages globally; always use the virtual environment
- Standard Python import statements: `import package` or `from package import module`

## Integration Points
- External dependencies installed via PyPI through pip
- No cross-component communication as this is an environment setup

Reference: `pyvenv.cfg` for Python version and paths.