# Triangle de Pascal - application console C++

Cette application C++ affiche les premieres lignes du triangle de Pascal dans la console. Par defaut, elle affiche 24 lignes.

## Fonctionnement

Une valeur a la ligne `n` et a la position `k` est un coefficient binomial :

```text
C(n, k) = n! / (k! * (n - k)!)
```

Le programme calcule ces coefficients de maniere iterative, sans calculer directement les factorielles.

## Prerequis

- Visual Studio 2022, ou une version compatible ;
- la charge de travail **Developpement Desktop en C++** ;
- MSVC v143 et le SDK Windows 10, configures dans le projet.

## Compiler et executer

1. Ouvrez `ConsoleApplicationPascalTriangle.sln` dans Visual Studio.
2. Choisissez une configuration (`Debug` ou `Release`) et une plateforme (`x64` ou `Win32`).
3. Compilez et lancez avec `F5` ou `Ctrl+F5`.

Le triangle est affiche dans la console. Le programme attend ensuite une touche avant de se fermer.

## Exemple de sortie

```text
 1
 1 1
 1 2 1
 1 3 3 1
 1 4 6 4 1
```

## Changer le nombre de lignes

Dans `ConsoleApplicationPascalTriangle/ConsoleApplicationPascalTriangle.cpp`, modifiez la valeur de `n` dans la fonction `main` :

```cpp
int n = 24;
```

## Limites

Les valeurs sont stockees dans un `long long`. Un nombre de lignes trop important peut donc provoquer un depassement d'entier.

## Licence

Ce projet est distribue sous licence MIT. Consultez [LICENSE.txt](LICENSE.txt).
