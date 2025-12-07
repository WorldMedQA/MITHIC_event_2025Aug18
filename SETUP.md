# Setup Instructions

## Quick Start

### 1. Install uv

**macOS/Linux:**
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

**Windows:**
```powershell
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
```

### 2. Setup Environment

```bash
# Create and activate virtual environment
uv venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# Install packages
uv pip install jupyter ipykernel pandas numpy matplotlib huggingface_hub
```

### 3. Create Jupyter Kernel

```bash
python -m ipykernel install --user --name=mithic --display-name="MITHIC"
```

### 4. Open Notebook

```bash
jupyter notebook MITHIC_event_2025Aug18.ipynb
```

Select Kernel → Change Kernel → MITHIC

## Troubleshooting

**"Command not found: uv"** - Restart terminal after install

**"No module named..."** - Make sure `.venv` is activated

**Kernel not showing** - Run the ipykernel install command again