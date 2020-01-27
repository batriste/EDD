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

archetype:generate: Indiquem que volem executar un col·leccio d'objectius amb proposit comú.
DgroupId:  l'identificador únic de l'organitzció que crea el projecte.
DartifactID: Indica el nom del recurs (artifact) que anem a generar.
DarchetypeArtifactId: Indica la plantilla per al nostre projecte.
DinteractiveMode: Indica si volem utilitzar o no el mode interactiu.

Una volta ejecutem el comandament es creara el fitxer pom.xml

### 2. Compilació del la estructura

Una vegada tenim la aplicacio el que farem sera contruir el projecte desde l'arrel(a on se encontra el fitxer pom)

```
mvn compile
```

Ara añadim el tarjet per a dirli a on te que ejecutar el programa desde la arrel
```
java -cp target/classes com.ieseljust.edd.App
```

Ara si vole empaquetar el nostre projecte en un .jar i netejar la carpeta del target anterior
```
mvn clean package
```