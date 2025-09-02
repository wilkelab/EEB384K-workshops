## Workshop overview

In this class we'll go over the basics of setting up a working python environment, edit code, manage dependencies, etc. You will do this on your own laptop, as it's important to know how to run things locally. In general, this will require (i) a python installation, (ii) Visual Studio Code, and (iii) a terminal app. If you routinely use these technologies you're probably already all set. If not, installation instructions are at the bottom of this page. It's much easier to set things up on a Mac than on Windows, but it is possible to set things up properly on Windows also.


## Creating a python virtual environment, installing dependencies, starting Jupyter

In a terminal, download the workshop materials, unzip, and navigate into the workshop folder:
```sh
wget https://github.com/wilkelab/EEB384K-workshops/archive/refs/heads/main.zip
unzip main.zip
cd EEB384K-workshops-main/week2
```

Note: We're deliberately not using `git clone` because VS Code gets confused if it sees a top-level git repository but python environments in subfolders, which is what we're doing here.


Create a python virtual environment:
```sh
python3 -m venv .venv
```

Activate the environment:
```sh
source .venv/bin/activate
```

Install the requirements:
```sh
pip install -r requirements.txt
```

Deactivate the environment:
```sh
deactivate
```

Now everything is set up properly. Next go to VS Code and open the folder for week2. (Do not open the parent folder! VS Code will not find the python virtual environment if you open the parent folder.) Then open the notebook `week2.ipynb` and follow the instructions there.
 

## Installation instructions for Mac

1. Install python

You can use homebrew if you're using it already, or otherwise install python from here: https://www.python.org/downloads/macos/Links to an external site.

2. Install VS Code and the python extension

Download from here: https://code.visualstudio.com/Links to an external site.

Then install the official Microsoft python extension and the Jupyter extension in VS Code.

3. Locate your terminal app

The terminal app, called "Terminal", can be found in the Utilities folder in Applications. You may find it helpful to drag it into the dock, as you may need it frequently for various things we'll do in this class.
 

## Installation instructions for Windows

On Windows, to make your experience bearable, you need to install the Windows Subsystem for Linux (WSL). You can find the relevant instructions here: https://learn.microsoft.com/en-us/windows/python/web-frameworks. Follow them up to and including the subsection "Install the Microsoft Python extension". It walks you through all the relevant steps, including installing python and VS Code.

Finally, install the Jupyter extension in VS Code.

 