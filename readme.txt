******IMPORTANTE  ANTE CUALQUIER INSTALACION CERRAR Y VOLVER A ABRIR EL BASH DE UBUNTU**********

*wsl --install
*Puede ser necesario en algunos casos, activar la virtualización del sistema, para ello hay que acceder a la BIOS y activar la virtualización desde ahí.
Para ello, abrimos PowerShell como administrador y usamos el siguiente comando (el mismo reiniciará nuestra PC y entrará a la BIOS: 
shutdown /r /fw

*NVM
**curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
**nvm install 14.7.0
**nvm install --lts
**comandos utiles
***Comandos utiles:     nvm list      |      nvm use <version>

*FNM
**sudo apt-get install unzip
**curl -fsSL https://fnm.vercel.app/install | bash
**fnm install 14.7.0
**fnm install --lts
**Comandos utiles:     fnm list      |      fnm use <version>

*GIT
**sudo apt-get install git
**git config --global user.name "Your Name"
**git config --global user.email "youremail@domain.com"
*Crear llave SSH
**ls-a para ver documentos ocultos
** rm -r .git/ para eliminar un repositorio o directorio
**cd .ssh/
*ls -al ~/.ssh para verificar si ya tenemos una clave ssh creada. Crear solo una por pc
**ls
**ssh-keygen -t ed25519 -C “email@example.com” ??????????????(la clave ed25519)
**cat id_ed25519
**Copiar lo que genera 
b3BlbnNzaC1rZXktdjEAAAAABG5vbmUAAAAEbm9uZQAAAAAAAAABAAAAMwAAAAtzc2gtZW
QyNTUxOQAAACDv/FBZV+nx2YvqZrtVOlg16xUZrb+vIDd/3rvfHy5y4wAAAKCefr7Onn6+
zgAAAAtzc2gtZWQyNTUxOQAAACDv/FBZV+nx2YvqZrtVOlg16xUZrb+vIDd/3rvfHy5y4w
AAAECRKE5i60Fyc9abYpsDKLnoYl3KMzNOI50ch87RmaYDL+/8UFlX6fHZi+pmu1U6WDXr
FRmtv68gN3/eu98fLnLjAAAAGGFsZWphbmRyb2lzYTcxQGdtYWlsLmNvbQECAwQF

*ir github => settings => SSh an GPG keys

*OTRO PC
**ssh-keygen
**Ir a github y poner nuevo key
**pegar lo generado