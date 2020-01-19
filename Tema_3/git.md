#git
###1. entrem en el directori ./git/ que hem creat on vuigam
cd /Escriptori
mkdir git
###2. Per a crear la base de dades de eixa carpeta farem us del git init
git init
###3. añadim el nostre usuari i gmail per poder modificar el nostre directori
git config --global user.name "nom"
git config --global user.email "correu_electronic"
###4. abams de crear un archiu tindrem que añadir els canvis del nostre servidor
git pull
###3. per crear un ficher but i añadirlo a git fem 
git add * per añadir tots els archius 
git add "nom_fitxer" per añadir sols eixe fitxer
###4. comprovem com esta el estat de git
git status
###5. añadim un comentari per fer una versio de git
git commit -a -m "mensaje"
###6. pujem els canvis que hem fet
git push