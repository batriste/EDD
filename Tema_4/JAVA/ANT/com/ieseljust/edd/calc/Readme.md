# GCC
## Compilacio ANT
Anem a crear primer els archius necesaris per generar Calcula.class i Calculadora.class

### 1. Anem a crear els archius Calcula.java i Calculadora.java

Calcula.java tindra implementat les funcions principals i fara us de les llibreries que hem creat.
Calculadora.java tindra les llibreries que cridarem.

### 2. Creem el un archiu build.xml per poder definir les fases de construccio

Hem de crear un archiu amb visual studio code per poder definir com se compilara el programa

### 3. Compilem el archiu Calcula.java i Calculadora.java per obtindre el abre de .class amb els archius

Desde la terminal i l'arrel del programa compilarem els archius 
```
$ javac com/ieseljust/edd/calc/*.java
```

### 4. Ara ejecutem per termial desde la arrel del programa

Ejecutem el programa fen us de ant

El comandament seria aixina
```
ant run -Darg0=3 -Darg1=4
```

#### 4.1 Explicacio
ant: Es el programa
run: Es per fer que se ejecute
-Darg0=1: Es el primer argument que hem indicat en el archiu
-Darg1=1: Es un altre argument per a que els compare

