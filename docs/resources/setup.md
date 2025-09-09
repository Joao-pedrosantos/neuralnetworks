# Tools & Setup Guide

## Required Software

### Python Environment
- **Python 3.8+** (recommended: Python 3.10 or 3.11)
- **Jupyter Notebook** or **JupyterLab**
- **Git** for version control

### Package Management
We recommend using **conda** or **pip** with virtual environments.

## Installation Instructions

### Option 1: Using Conda (Recommended)

```bash
# Create a new environment
conda create -n neural-networks python=3.10

# Activate the environment
conda activate neural-networks

# Clone the repository
git clone https://github.com/joao-pedrosantos/neuralnetworks.git
cd neuralnetworks

# Install packages
conda install jupyter numpy matplotlib pandas scikit-learn
pip install -r requirements.txt
```

### Option 2: Using pip with venv

```bash
# Create virtual environment
python -m venv neural-networks-env

# Activate environment (Windows)
neural-networks-env\Scripts\activate

# Activate environment (macOS/Linux)
source neural-networks-env/bin/activate

# Clone and install
git clone https://github.com/joao-pedrosantos/neuralnetworks.git
cd neuralnetworks
pip install -r requirements.txt
```

## Required Python Packages

The main packages you'll need:

```text
numpy>=1.21.0          # Numerical computing
matplotlib>=3.5.0      # Plotting and visualization  
pandas>=1.3.0          # Data manipulation
jupyter>=1.0.0         # Interactive notebooks
scikit-learn>=1.0.0    # Machine learning utilities
seaborn>=0.11.0        # Statistical visualization
```

## Development Environment

### Jupyter Setup

Launch Jupyter from your project directory:

```bash
# Start Jupyter Notebook
jupyter notebook

# Or start JupyterLab (recommended)
jupyter lab
```

### VS Code (Optional)

If you prefer VS Code:
1. Install the Python extension
2. Install the Jupyter extension
3. Open the project folder
4. Select your Python interpreter (conda/venv environment)

## Troubleshooting

### Common Issues

!!! warning "Import Errors"
    If you get `ModuleNotFoundError`:
    
    1. Make sure your environment is activated
    2. Install missing packages: `pip install package-name`
    3. Restart Jupyter kernel

!!! warning "Jupyter Not Starting"
    Try these solutions:
    
    - Check if port 8888 is already in use
    - Start on a different port: `jupyter notebook --port 8889`
    - Clear browser cache and cookies

### Package Version Conflicts

If you encounter version conflicts:

```bash
# Check installed packages
pip list

# Upgrade specific package
pip install --upgrade package-name

# Fresh installation
pip uninstall package-name
pip install package-name
```

## Hardware Requirements

### Minimum Requirements
- **RAM**: 8GB (16GB recommended)
- **Storage**: 2GB free space
- **CPU**: Modern multi-core processor

### For Advanced Exercises
- **GPU**: NVIDIA GPU with CUDA support (optional but helpful)
- **RAM**: 16GB+ for larger datasets

## Testing Your Setup

Run this test to verify everything works:

```python
# test_setup.py
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
import sklearn

print("✅ NumPy version:", np.__version__)
print("✅ Matplotlib version:", plt.matplotlib.__version__)
print("✅ Pandas version:", pd.__version__)
print("✅ Scikit-learn version:", sklearn.__version__)

# Create a simple plot
x = np.linspace(0, 10, 100)
y = np.sin(x)
plt.plot(x, y)
plt.title("Setup Test - Sine Wave")
plt.show()

print("🎉 Setup complete!")
```

## Additional Tools

### Optional but Helpful

- **Git GUI**: GitKraken, Sourcetree, or GitHub Desktop
- **Text Editor**: VS Code, PyCharm, or Sublime Text
- **Documentation**: Access to this course website
- **Calculator**: For manual verification of calculations

## Getting Help

If you encounter setup issues:

1. **Check the FAQ**: Common solutions are in [FAQ](faq.md)
2. **GitHub Issues**: Create an issue in the course repository
3. **Community**: Use the Discussions tab on GitHub
4. **Documentation**: Refer to official package documentation

## Next Steps

Once your environment is set up:

1. **Test with a simple exercise**: Try [Exercise 1A](../exercises/exercise1/part-a.md)
2. **Explore the repository**: Familiarize yourself with the structure
3. **Read the course overview**: Check [Course Overview](../index.md)
4. **Join discussions**: Engage with other students on GitHub

---

**Happy coding!** 🚀