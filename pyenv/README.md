# 🐍 Python Environment Setup with pyenv

A comprehensive guide to setting up Python development environment using pyenv.

## 📋 Prerequisites

- Linux/macOS system
- Bash shell
- Internet connection

## 🚀 Quick Installation

### Step 1: Install pyenv
```bash
# Download and install pyenv
curl https://raw.githubusercontent.com/Neo2Go/install-server/main/install-pyenv.sh | bash

# Reload shell configuration
source ~/.bashrc
```

### Step 2: Install Python Version
```bash
# Install Python 3.9.6
pyenv install 3.9.6

# Set as global Python version
pyenv global 3.9.6
```

### Step 3: Create Virtual Environment
```bash
# Create a virtual environment named 'chrenv'
pyenv virtualenv 3.9.6 chrenv

# Set as local environment for current project
pyenv local chrenv
```

## 🔧 Useful Commands

| Command | Description |
|---------|-------------|
| `pyenv versions` | List all installed Python versions |
| `pyenv version` | Show current active Python version |
| `pyenv install --list` | List all available Python versions |
| `pyenv virtualenv <version> <name>` | Create new virtual environment |
| `pyenv activate <env-name>` | Activate virtual environment |
| `pyenv deactivate` | Deactivate current environment |

## 📝 Environment Management

### Create Additional Environments
```bash
# For different projects
pyenv virtualenv 3.9.6 project-name
pyenv virtualenv 3.11.0 modern-project
```

### Switch Between Environments
```bash
# Activate specific environment
pyenv activate chrenv

# Set local environment for project
cd /path/to/project
pyenv local chrenv
```

## 🛠️ Troubleshooting

### Common Issues

1. **Command not found**: Ensure pyenv is in your PATH
   ```bash
   echo 'export PATH="$HOME/.pyenv/bin:$PATH"' >> ~/.bashrc
   echo 'eval "$(pyenv init -)"' >> ~/.bashrc
   source ~/.bashrc
   ```

2. **Build dependencies**: Install required packages
   ```bash
   # Ubuntu/Debian
   sudo apt-get update
   sudo apt-get install make build-essential libssl-dev zlib1g-dev \
   libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm \
   libncursesw5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev
   ```

## 📚 Additional Resources

- [pyenv Documentation](https://github.com/pyenv/pyenv)
- [Python Virtual Environments Guide](https://docs.python.org/3/tutorial/venv.html)
- [Best Practices for Python Development](https://python-guide.readthedocs.io/)

---

**Happy Coding! 🎉**
