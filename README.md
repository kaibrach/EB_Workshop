# EB_Workshop
Elektrobit Workshop Neural Networks

Start tensorflow container with jupyter notebooks in cmd/Powershell:
1. docker pull schmiederx/workshop:latest
2. navigate to the directory of the workshop folder 
3. docker run -it --rm -v "$(pwd):/tf" -p 8888:8888 -p 6006:6006 schmiederx/workshop:latest