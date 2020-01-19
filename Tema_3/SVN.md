#SVN
Per poder treballar de manera conjunta en altre programadors tindrem que portar un control de versions per saber quins canvis ha realitzat cadascun, de eixa necessitat sorgeix el control de versions centralitzat amb un unic servidor que emmagatzeme les diferents versions dels fitxers.
###1. Instalacio de subversion client
sudo apt install subversion
###2. Per a crear un repositori accedim desde el navegador a localhost
http://localhost:18080
dins del mateix crearem un repositori
###3. Descarregem la ultima versio del nostre repositori
amb el comando svn co fem un de check out del repositori
 svn co http://localhost:18080/svn/Projecte1 --username=joamuran
###3. Creem un fitxer anomenat exemple1.js
primer entrem a el nostre repositori i despres creem el archiu en la carpeta trunk
vim exemple1.js
dins de aques archiu añadim 
1 function saluda(){
2 console.log("Hola Subversion");
3 }saluda()
estem en el directori Projecte1/trunk
###4. Provem a executarlo el codic amb nodejs
nodejs trunk/exemple1.js
###5. Comprovem els canvis del nostre repositori
Per comprovar els canvis farem us de svn i per saber el estat st
svn st 
###5. Añadim els canvis al control de versions 
svn add trunk/exemple1.js
svn ci -m "Afegint fitxer exemple1.js"
svn up
