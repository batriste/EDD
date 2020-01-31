# GCC
## Compilacio GRADLE

### Requisits:

Tindre els fitxers Calcula i Calculadora.

Tindre instalat gradle.
```
$ sudo apt-get update

$ sudo apt-get install gradle
```

### 1. En primer lloc projecte GRADLE

Començarem iniciant el projecte
```
$ gradle init
```

Triarem les opcions:
· Type: 4
· Build: 1
· Test framework: 1
· Name: Calcula
· Source package: com.ieseljust.edd

### 2. Modifiquem el archiu build.gradle

Per poder contruir el projecte tindrem que modificar l'ultima linea per cambiar el main class

De
```
mainClassName = 'com.ieseljust.edd.App'
```
A
```
mainClassName = 'com.ieseljust.edd.Calcula'
```

### 3. Contrucció i execució

Fent us del comandament build crearem el projecte
```
$ gradle build
```
Amb gradle run llancarem el programa