
# Conda (Python) – Installation & Virtual Environment
## What is Conda?
Conda is a package, dependency, and environment manager for Python and system-level libraries.

---

## Install Conda on macOS

### Install using Homebrew:
```bash
brew install --cask anaconda
```

### Initialize Conda:
```bash
conda init "$(basename "${SHELL}")"
```

### Reload shell:
```bash
source ~/.zshrc  
```

### Verify installation:
```bash
conda --version
```

---

## Update Conda
```bash
conda update conda
```

---

## Create a Virtual Environment

### Default:
```bash
conda create --name myenv
```

### Specific Python version:
```bash
conda create --name myenv python=3.12
```

### With packages:
```bash
conda create --name mlenv python=3.10 numpy pandas scikit-learn
```

---

## Activate / Deactivate Environment

### Activate:
```bash
conda activate myenv
```

### Deactivate:
```bash
conda deactivate
```

---

## Remove an Environment
```bash
conda remove --name myenv --all
```

---

## Package Management

### Install package:
```bash
conda install numpy
```

### Install from conda-forge:
```bash
conda install -c conda-forge tensorflow
```

### Update:
```bash
conda update pandas
```

### Remove:
```bash
conda remove numpy
```

### List packages:
```bash
conda list
```

---

## Manage Channels

### Show channels:
```bash
conda config --show channels
```

### Add conda-forge:
```bash
conda config --add channels conda-forge
```

---

## Export & Import Environment (YAML)

### Export:
```bash
conda env export > environment.yaml
```

### Create from YAML:
```bash
conda env create -f environment.yaml
```
