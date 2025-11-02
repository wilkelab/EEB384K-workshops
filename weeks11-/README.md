## Creating a python virtual environment, installing dependencies, starting Jupyter

In a terminal, download the workshop materials, unzip, and navigate into the workshop folder:
```sh
wget https://github.com/wilkelab/EEB384K-workshops/archive/refs/heads/main.zip
unzip main.zip
cd EEB384K-workshops-main/weeks11-
```

Note: We're deliberately not using `git clone` because VS Code gets confused if it sees a top-level git repository but python environments in subfolders, which is what we're doing here.

Then create a python virtual environment and install all the requirements:
```sh
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
deactivate
```

Now everything is set up properly. Next go to VS Code and open the folder for weeks11-. (Do not open the parent folder! VS Code will not find the python virtual environment if you open the parent folder.) Then open the notebook `week11.ipynb` (for week 11) and follow the instructions there.
