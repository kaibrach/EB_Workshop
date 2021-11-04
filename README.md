# EB_Workshop
Elektrobit Workshop on Neural Networks


# 1. Clone or Download the repository
1. Create a workshop folder e.g. `C:\tmp\Workshop`
> Clone: `git clone https://github.com/kaibrach/EB_Workshop.git`

OR

> Download (no Git installed): `https://github.com/kaibrach/EB_Workshop/archive/main.zip`


# 2. Prepare your System
You can either choose to create a **virtual environment (recommended)** or use a **docker** file.
## 2.1 Using Virtual Environment

### Step 1. Installation
> 1. We assume that you have installed python version 3.7 on your windows machine.    
   [Download Python 3.7.9 (64 Bit)](https://www.python.org/ftp/python/3.7.9/python-3.7.9-amd64-webinstall.exe)

### Step 2. Create Environment
> 2. Open Console or Powershell and navigate to the directory of the workshop folder e.g. `cd C:\tmp\Workshop`

> 3. Run `python -m venv eb_workshop-env` 

> 4. Once you’ve created a virtual environment, you may activate it `eb_workshop-env\Scripts\activate`

> 5. Install all necessary python packages `pip install -r requirements.txt`

### Step 3. Run Jupyter Notebook
> 6. Create a Jupyter Kernel with `python -m ipykernel install --user --name EB_WORKSHOP --display-name "EB Workshop"`    
    The --name value is used by Jupyter internally. These commands will overwrite any existing kernel with the same name. --display-name is what you see in the notebook menus.

> 7. Run `jupyter notebook` from console


## 2.2 Using Docker

### Step 1. Installation
> 1. Install docker desktop     
[Download Docker_Desktop](https://desktop.docker.com/win/stable/Docker%20Desktop%20Installer.exe)       
 --> Make sure you have virtualization (Hyper-V) enabled in your BIOS

### Step 2. Create Environment
> 2. Start Windows Powershell

> 3. run command `docker pull schmiederx/workshop:latest`

### Step 3. Run Jupyter Notebook
Start tensorflow container with jupyter notebooks in cmd/Powershell:

> 4. Open Windows `Powershell` and navigate to the directory of the workshop folder e.g. `cd C:\tmp\Workshop`

> 5. Run `docker run -it --rm -v "$(pwd):/tf" -p 8888:8888 -p 6006:6006 schmiederx/workshop:latest`

> 6. Copy the `http://127.0.0.1/?token=xxxxxxxxx` link from the command line and paste into webrowser address bar
