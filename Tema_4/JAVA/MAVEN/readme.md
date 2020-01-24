# GCC
## Compilacio Maven

### 1. Generar el projecte a partir de l'estructura

Primer el que farem es obrir un terminal i comprovem que tenim maven instalat

```
$ sudo apt update
$ sudo apt install maven
$ mvn --version
```

Una volta tenim comprovat que tenim Maven instalat començem amb el projecte.

```
mvn archetype:generate -DgroupId=com.ieseljust.edd -DartifactId=CalculaMVN -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
```

archetype:generate:
DgroupId:
DartifactID:
DarchetypeArtifactId:
DinteractiveMode:

### 2. Compilació del la estructura

Una vegada tenim la aplicacio el que farem sera contruir el projecte

```
mvn compile
```

Ara añadim el tarjet per a dirli a on te que ejecutar el programa desde la arrel
```
java -cp target/classes com.ieseljust.edd.App
```