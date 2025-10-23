git config --global user.name "Tu Nombre"
git config --global user.email "correo@correo.com"
git config --list

 
ssh-keygen -t ed25519 -C "correo@correo.com"
sc config ssh-agent start=auto
net start ssh-agent
ssh-add %userprofile%\.ssh\id_ed25519
 
 type %USERPROFILE%\.ssh\id_ed25519.pub | clip


 ssh git@github.com -T