# GCC
Anem a crear primer els archius necesaris per generar calcula.

### 1. Anem a crear els archius calc.c i calc.h

calc.c tindre implementat les funcions
calc.h tindra la capçalera(suma, resta, multiplica, divideix)

### 2. Compilem el archiu calc.c per obtindre el archiu.o

```
gcc -c calc.c -o calc.o
```


### 3. Creem el fitxer executable calcula a partir dels dos fitxers

    gcc -Wall -g calcula.c calc.o -o calcula