#RCS
###1. Creeu un fitxer anomenat exercici.md, i afegiu-li algun contingut en format Markdwon.
vim exercici.md
añadim contingut
###2. Registreu el fitxer per a que el controle RCS.
amb ci -u "nom archiu" añadim el ficher al RCS
###3. Intenteu modificar el fitxer, per veure si teniu o no permís.
amb ls -l vorem que no tenim permisos sols -r--r--r--
###4. Feu un checkout del fitxer, ara sí, per afegir canvis.
amb co -l "archiu" podrem afegir canvis al archiu(ens dona permis de escriptura sols per al usuari)
###5. Modifiqueu el fitxer i afegiu-li més contingut. Aquesta serà la versió 1.2.
####Per a poder escriure ara dins del archiu farem us del nano, vim, touch
nano exercici.md 
####Ara tornem a añadir el archiu al rcs amb ci -u
ci -u exercici.md 
###6.Revisa la versio de exercici.md
amb rlog ./exercici.md podem vore les versions del archiu
