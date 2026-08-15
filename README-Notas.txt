# Acá está el material compartido en Drive
https://drive.google.com/drive/shared-with-me

# Acá Encontré el Jupyter NB de la clase
https://cienciadedatos.net/documentos/pystats06-analisis-normalidad-python

# El paraíso para Ciencia de Datos en Python
https://cienciadedatos.net/

#@title Clone GitHub Repository into Google Colab Sample

# Replace with your GitHub username and repository name
GITHUB_USERNAME = "zetaware" #@param {type:"string"}
GITHUB_REPOSITORY_NAME = "estadistica_con_python" #@param {type:"string"}

# If your repository is private, uncomment the following line and replace 'github_token' with the name of your secret
# from google.colab import userdata
# GITHUB_TOKEN = userdata.get('github_token') # Store your GitHub PAT as a secret named 'github_token'

# Construct the repository URL. Use a PAT for private repositories.
# if 'GITHUB_TOKEN' in locals() and GITHUB_TOKEN:
#     github_url = f"https://{GITHUB_USERNAME}:{GITHUB_TOKEN}@github.com/{GITHUB_USERNAME}/{GITHUB_REPOSITORY_NAME}.git"
# else:
github_url = f"https://github.com/{GITHUB_USERNAME}/{GITHUB_REPOSITORY_NAME}.git"

# Clone the repository
!git clone {github_url}

print(f"Repository '{GITHUB_REPOSITORY_NAME}' cloned successfully!")
