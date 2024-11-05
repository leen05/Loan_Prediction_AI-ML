import subprocess
import sys

# Check if the package is installed, if not, install it
try:
    import imblearn
except ImportError:
    subprocess.check_call([sys.executable, "-m", "pip", "install", "-U", "imbalanced-learn"])
