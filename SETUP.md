# Project setup — what to create first

Do these in order.

---

## 1. Create the environment (do this first)

You have two options. Use **one** of them.

### Option A — Conda (recommended if you use Anaconda/Miniconda)

```bash
# Create environment with Python 3.11
conda create -n jb_freight python=3.11 -y

# Activate it
conda activate jb_freight
```

### Option B — venv (built into Python)

```bash
# From project folder: c:\Users\kanam\OneDrive\Desktop\jb
python -m venv venv

# Activate it (Windows PowerShell)
.\venv\Scripts\Activate.ps1
```

---

## 2. Install packages

With the environment **activated**:

```bash
pip install -r requirements.txt
```

---

## 3. Use this environment in your notebook

- **Conda:** If you created `jb_freight`, in Jupyter choose kernel: `jb_freight` (or run `python -m ipykernel install --user --name jb_freight` once).
- **venv:** Select the kernel that points to `venv\Scripts\python.exe`.

---

## Summary order

| Step | What to do |
|------|------------|
| 1 | Create environment (conda or venv) |
| 2 | Activate it |
| 3 | `pip install -r requirements.txt` |
| 4 | Open the notebook and pick this environment as the kernel |

After that you’re ready to run the notebook.
