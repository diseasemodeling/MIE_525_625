# JUPYTER HUB

### Login and LOGOUT of JupyterHub
Use the link on Canvas to access JupyterHub for classroom    
Login using UMass credentials (may ask only the first time)  
Select container image based on assignment needs 
Start server

LOGOUT: 
FILE --> HUbControlPanel --> STOP SERVER


### Clone GITHUB repo to your JupyterHub
git clone 'url_link_to_github_repo'

### Clone specific folders in repo to your JupyterHub. Example to clone A1_Graded
TERMINAL COMMANDS:  
git clone --no-checkout https://github.com/diseasemodeling/MIE_525_625.git  
cd MIE_525_625  
git sparse-checkout init --cone  
git sparse-checkout set A1_Graded  
git checkout main  
