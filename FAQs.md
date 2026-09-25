# JUPYTER HUB

### Login and LOGOUT of JupyterHub
Use the link on Canvas to access JupyterHub for classroom    
Login using UMass credentials (may ask only the first time)  
Select container image based on assignment needs 
Start server

BE SURE TO STOP SERVER (so it frees up compute space): 
FILE --> HUbControlPanel --> STOP SERVER

### Accessing files
* Uses typical route of download (from source say GITHUB repo to your local folder on your computer) and upload (from your computer folder to JupyterHub0
* Clone GITHUB repo
* wget to ACCESS ONE SINGLE FILE

### ACCESS ONE SINGLE FILE from GITHUB repo: wget url_link
  * example: "wget https://github.com/diseasemodeling/MIE_525_625/blob/main/Lectures/2d_Code_NN_PyTorch_Basic.ipynb"

### Clone GITHUB repo to your JupyterHub
git clone 'url_link_to_github_repo'

### Clone specific folders in repo to your JupyterHub. Example to clone A1_Graded
TERMINAL COMMANDS:  
git clone --no-checkout https://github.com/diseasemodeling/MIE_525_625.git  
cd MIE_525_625  
git sparse-checkout init --cone  
git sparse-checkout set A1_Graded  
git checkout main  

### Terminal commands for checking storage usage 
* Check overall usage: df -h ~   
* Check each file/folder size: du -sh ~/* ~/.* 2>/dev/null | sort -h   
* Check for specific folder, e.g., in folder "~/.cache/*" :  du -sh ~/.cache/* | sort -h    
* Check deeper into each subfolder, e.g.,: ls -lh ~/.cache/huggingface/hub/    
* To remove folder: rm -rf ~/.cache/huggingface/*  
