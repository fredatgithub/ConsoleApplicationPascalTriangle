# Triangle de Pascal — application console C++

Cette application C++ affiche les premières lignes du triangle de Pascal dans la console. Par défaut, elle en affiche 24.

## Principe

Chaque valeur du triangle correspond à un coefficient binomial :

```text
C(n, k) = n! / (k! × (n - k)!)
```

Les coefficients sont calculés de manière itérative, sans calculer directement les factorielles.

## Prérequis

- Visual Studio 2022 (ou version compatible) avec la charge de travail **Développement Desktop en C++** ;
- le jeu d’outils MSVC v143 et le SDK Windows 10, tels que configurés dans le projet.

## Compilation et exécution

1. Ouvrez `ConsoleApplicationPascalTriangle.sln` dans Visual Studio.
2. Sélectionnez la configuration souhaitée (`Debug` ou `Release`) et la plateforme (`x64` ou `Win32`).
3. Compilez et lancez le projet avec `F5` ou `Ctrl+F5`.

Le programme affiche le triangle, puis attend une entrée clavier avant de se fermer.

## Exemple de sortie

```text
 1
 1 1
 1 2 1
 1 3 3 1
 1 4 6 4 1
```

## Modifier le nombre de lignes

Dans `ConsoleApplicationPascalTriangle/ConsoleApplicationPascalTriangle.cpp`, modifiez la valeur de `n` dans `main` :

```cpp
int n = 24;
```

## Limite

Les valeurs sont stockées dans un `long long`. Pour un nombre de lignes élevé, les coefficients binomiaux peuvent dépasser sa capacité et provoquer un dépassement d’entier.

## Licence

Ce projet est distribué sous licence MIT. Consultez [LICENSE.txt](LICENSE.txt).
