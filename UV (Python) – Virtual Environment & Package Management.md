# **UV (Python) – Virtual Environment & Package Management**

## **What is uv?**

uv is a super-fast Python package manager and virtual environment tool.

It replaces pip, pipx, virtualenv, and sometimes even poetry workflows.

**Key features:** 

* Creates virtual environments

* Installs Python packages

* Manages multiple Python versions

* Extremely fast (written in Rust)

---
## **Install uv package using Homebrew on MacOS:**

### **Update Homebrew**

Always update brew before installing anything:
```
brew update
```

### **Install uv using Homebrew**
```
brew install uv
```

### **Verify Installation**
```
uv --version
```

---
## **Create a Virtual Environment**

### **Intialise the uv in the folder where you want to create the virtual environment**
```
uv init
```

### **Create a venv inside current folder:**
```
uv venv
```
This creates a folder .venv/ or myenv/.

---
## **Activate the Environment**

### **macOS:**
```
source .venv/bin/activate
```

or

```
source myenv/bin/activate
```

## **Deactivate Environment**

```
deactivate
```

---

# **Package Management (Using uv)**

### **Install a package:**
```
uv add requests
```

### **Install multiple packages:**
```
uv add numpy pandas
```

### **Install a specific version:**

```
uv add flask==3.0.0
```

### **Remove a package:**
```
uv remove requests
```

### **List installed packages:**
```
uv pip list
```

---
## **Requirements Management**

### **Freeze packages:**
```
uv pip freeze > requirements.txt
```

### **Install from requirements:**
```
uv pip install -r requirements.txt
```
---
## **Manage Python Versions with uv**

### **Install a python version:**
```
uv python install 3.12
```

### **Create venv with specific version:**
```
uv venv --python 3.12
```




