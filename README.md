# SAF_TP0_JAVA_EXO1-2-CALCULATOR

# TP0 - Introduction à Java/NetBeans et création d'une Calculatrice

Ce dépôt contient mes tout premiers pas en Java dans le cadre du cours de programmation à l'EFREI Paris. L'objectif était de prendre en main l'environnement NetBeans et de manipuler les bases du langage à travers trois fichiers.

---

## Bilan par Fichier

### 1. Fichier Exo1.java (Découverte de l'IDE)
Dans ce premier fichier, j'ai appris à configurer un projet et à utiliser l'auto-complétion. J'ai compris l'importance de mettre un cartouche d'identification en haut pour documenter mon nom, ma classe et mon enseignante. J'ai aussi appris à utiliser l'ampoule de correction pour importer automatiquement des outils comme java.util.Scanner.

### 2. Fichier Exo2.java (Bugs et Boucles)
Ce fichier servait à corriger un programme qui ne fonctionnait pas. J'ai analysé une boucle while pour corriger deux grosses erreurs : l'oubli de l'incrémentation du compteur (ind++ comme vu en cours), ce qui créait une boucle infinie. Cela m'a appris à bien tracer mes variables pour éviter les plantages.

### 3. Fichier Calculator.java (Le projet final)
C'est le gros morceau du TP où j'ai assemblé toutes les notions pour créer une calculatrice interactive :
* **Menu & Saisie :** Affichage des options (1 à 5) et récupération des choix et des nombres avec Scanner (int pour l'opération et double pour accepter les chiffres à virgule).
* **Conditions (if / else if) :** Utilisation d'une structure rudimentaire pour lier le choix de l'utilisateur au bon calcul mathématique (+, -, *, /, %).
* **Gestion des erreurs :** Optimisation du code pour vérifier l'opérateur tout de suite après sa saisie. Si le nombre n'est pas entre 1 et 5, le programme affiche une erreur et s'arrête immédiatement avec un return, sans demander les nombres pour rien.

---

## Ce que je retiens globalement
Ce premier TP m'a donné les bases de la logique et de l'interactivité en Java. Je retiens qu'un bon code doit être propre et documenté, mais surtout qu'il faut anticiper les erreurs de l'utilisateur dès le début pour rendre le programme robuste.

