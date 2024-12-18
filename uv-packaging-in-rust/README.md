# UV for Python
[docs](https://astral.sh/blog/uv)

## Installation

```bash
# On macOS using brew.
brew install uv
```

Or, from [PyPI](https://pypi.org/project/uv/):

```bash
# With pip.
pip install uv
```

```bash
# Or pipx.
pipx install uv
```

Or, from [The Rust Package Manager](https://github.com/rust-lang/cargo)

```bash
cargo install --git ...
```

Install uv with our standalone installers:

```bash
# On macOS and Linux.
curl -LsSf https://astral.sh/uv/install.sh | sh
```

If installed via the standalone installer, uv can update itself to the latest version:

```bash
uv self update
```

### Enable shell completion
```zsh
eval "$(uv generate-shell-completion zsh)"
```

## Set up a new project

```bash
# Create a Python app with pyproject.toml file - Default init.
uv init --app
```

```bash
# Create a source code file.
uv init --lib
```

```bash
# Create a Python package.
uv init --package
```

```bash
# Create a Python app with a custom name.
uv init my-app
```

### Running the app
```bash
# Create a virtual environment.
uv run hello.py
```

### Adding dependencies
```bash
uv add fastapi
```

```bash
# Add multiple dependencies
uv add pandas sqlmodel
```

### Removing dependencies
```bash
uv remove sqlmodel
```

### Sync dependencies 
```bash
uv sync
```

### Create explicitly uv.lock file
```bash
uv lock
```

### Upgrade a specific package
```bash
uv lock --upgrade package fastapi
```

### Show the dependencies tree
```bash
uv tree
```

### Create a workspace
```bash
uv init another-app
```

### Install tools
```bash
uv tool install ruff
```

### Uninstall tools
```bash
uv tool uninstall ruff
```

### Upgrade a specific tool
```bash
uv tool upgrade ruff
```

### Show the list of available Python versions
```bash
uv python list
```

### Install specific Python version
```bash
uv python install 3.13.0
```

```bash
# Install with constrains
uv python install '>=3.10,<3.11'
```

### Set up specific Python version
```bash
uv python install 3.13.0
```




