# EB_Workshop
Elektrobit Workshop Neural Networks

# Step 1: Installation
1. Install docker desktop [Docker_Desktop](https://desktop.docker.com/win/stable/Docker%20Desktop%20Installer.exe)
   * Make sure you have virtualization (Hyper-V) enabled in your BIOS
2. Download docker file
   1. Start Windows Powershell
   2. run command `docker pull schmiederx/workshop:latest`

# Step 2: Clone the repository
1. Create a workshop folder somewhere e.g. `C:\tmp\Workshop`
2. git clone https://github.com/kaibrach/EB_Workshop.git

# Step 3: Start Jupyter Notebook 
Start tensorflow container with jupyter notebooks in cmd/Powershell:
1. Open Windows Powershell
2. navigate to the directory of the workshop folder 
3. `docker run -it --rm -v "$(pwd):/tf" -p 8888:8888 -p 6006:6006 schmiederx/workshop:latest`
4. Copy the http link from the command line and past it to the webrowser
