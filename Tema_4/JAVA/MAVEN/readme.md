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

### 2. Modifiquem el fitxer pom.xml

Dins de l'archiu pom.xml anyadirem despres de on s'indica la url de maven.apache.org
```
  <properties>
    <maven.compiler.source>1.6</maven.compiler.source>
    <maven.compiler.target>1.6</maven.compiler.target>
  </properties>
```

### 3. Compilació del la estructura

Una vegada tenim l'aplicacio el que farem sera construir el projecte desde l'arrel (a on se encontra el fitxer pom.xml)

```
$ mvn compile
```

Ara anyadim el objectiu per a dirli a on te que ejecutar el programa desde l'arrel i passar-li les dades
```
$ java -cp target/classes com.ieseljust.edd.Calcula 3 4
```

Ara si vole empaquetar el nostre projecte en un .jar i netejar la carpeta del target anterior
```
$ mvn clean package
```