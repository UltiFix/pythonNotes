# VSCode python extensions
- Python
- Pylance
- Python Debugger
- Python Environments

# VSCode create VENV
Ctrl + Shift + P
Type: Python: Create Environment

# VSCode set up VENV terminal activation
Ctrl + ,
Search for: Activate environment
Check the boxes for:
Python > Terminal: Activate Environment
Python > Terminal: Activate Env In Current Terminal
Python-envs > Terminal: Show Activate Button


# Build EXE
ensure venv activated in terminal
pip install pyinstaller
pyinstaller --onefile --name "GrbDiffCompiled-$(git rev-parse --short HEAD)-$(git show -s --format=%cd --date=format:%Y%m%d-%H%M%S)" GrbDiff.py
