#Visual_Studio_Code
Per a poder obtindre VS Code e instalarlo tenim que fer el seguent:
1. Obtenim la Clau GPG amb la que estan signats els paquets per a poder añadirlos al sistema.
1.1 $ curl https://packages.microsoft.com/keys/microsoft.asc | gpg --
dearmor > packages.microsoft.gpg
1.2 $ sudo install -o root -g root -m 644 packages.microsoft.gpg /usr/share
/keyrings/
2. Creem el fitxer vscore.list per a poder añadir al repositori:
2.1 $ sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/
repos/vscode stable main" > /etc/apt/sources.list.d/vscode.list'
2.2 $ sudo sh -c 'echo "deb [arch=amd64 signed-by=/usr/share/keyrings/
packages.microsoft.gpg] https://packages.microsoft.com/repos/vscode
stable main" > /etc/apt/sources.list.d/vscode.list'
3. ara instalem els paquets.
3.1 sudo apt-get install apt-transport-https
3.2 sudo apt-get update
3.3 sudo apt-get install code
4. Ara anirem a instalar extensions
![Javaxp](https://github.com/batriste/EDD/blob/master/imagenes/java.png)
Farem click en instalar
4.1 javac -version
5. Comprovem quines versions de jdk tenim instal·lades
en el cas de no tindre versio instala farem:
5.1 sudo apt install default-jdk
5.2 sudo apt install openjdk-11-jdk-headless
5.3 sudo apt install ecj
5.4 sudo apt install openjdk-8-jdk-headless
5.5 sudo apt install openjdk-9-jdk-headless
6.Vore el fitxet
añadim la linea  "java.json": "/usr/lib/jvm/java-11-openjdk-amd64"
![Javaxp](https://github.com/batriste/EDD/blob/master/imagenes/javajson.png)