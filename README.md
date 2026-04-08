<div style="margin-top:30px; text-align:center;">
  <img src="https://skillicons.dev/icons?i=html,css,js" />
</div>

<div style="text-align:center; margin-top:30px;">
<a href="#"><img src="https://img.shields.io/badge/LinkedIn-00f7ff?style=for-the-badge&logo=linkedin&logoColor=black"></a>
<a href="#"><img src="https://img.shields.io/badge/Email-ff0077?style=for-the-badge&logo=gmail&logoColor=white"></a>
</div>
{
    "name": "GitHub Readme Stats Dev",
    "image": "mcr.microsoft.com/devcontainers/base:ubuntu",
    "features": {
        "ghcr.io/devcontainers/features/node:1": { "version": "22" }
    },
    "forwardPorts": [3000],
    "portsAttributes": {
        "3000": { "label": "HTTP" }
    },
    "appPort": [],

    postCreateCommand' to run commands after the container is created.
    "postCreateCommand": "npm install -g vercel",

    Use 'postStartCommand' to run commands after the container is started.
    "postStartCommand": "hostname dev && npm install",
    // Configure tool-specific properties.
    "customizations": {
        "vscode": {
            "extensions": [
                "yzhang.markdown-all-in-one",
                "esbenp.prettier-vscode",
                "dbaeumer.vscode-eslint",
                "github.vscode-github-actions"
            ]
        }
    },

    "remoteUser": "root",
    "privileged": true
}
