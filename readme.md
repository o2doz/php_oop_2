## 📋 Exercice 1 : La classe Joueur

### Énoncé

Créez une classe `Joueur` qui représente un joueur de football avec les caractéristiques suivantes :

**Propriétés requises :**
- Un identifiant unique (numéro de joueur)
- Le prénom du joueur
- Le nom du joueur
- La position sur le terrain (exemple : "Attaquant", "Milieu de terrain", "Défenseur", "Gardien")
- Le numéro du maillot
- L'année de naissance

**Constructeur :**
- Doit initialiser toutes les propriétés lors de la création d'une instance
- Les paramètres doivent être passés dans cet ordre : numéro, prénom, nom, position, maillot, année de naissance

**Méthodes :**
- Une méthode pour retourner les informations complètes du joueur sous forme de texte
- Une méthode pour retourner l'âge du joueur (calculé à partir de l'année de naissance et l'année actuelle)
- Une méthode pour changer la position du joueur
- Une méthode pour afficher le profil du joueur de manière formatée (par exemple : "Nom : ..., Position : ..., Âge : ...")

**Règles de visibilité :**
- Les propriétés doivent être `private` (privées)
- Les méthodes doivent être `public` (publiques)
- Créez des méthodes getter pour accéder aux propriétés depuis l'extérieur

### Travail à faire

1. Créez le fichier `Joueur.php`
2. Déclarez la classe et ses propriétés
3. Écrivez le constructeur
4. Implémentez toutes les méthodes requises
5. Testez votre classe en créant 3 instances de joueurs différents
6. Appelez les différentes méthodes pour vérifier qu'elles fonctionnent correctement

---

## 📋 Exercice 2 : La classe Equipe

### Énoncé

Créez une classe `Equipe` qui représente une équipe de football.

**Propriétés requises :**
- L'identifiant de l'équipe
- Le nom de l'équipe
- La ville d'origine
- L'entraîneur (nom)
- Une liste de joueurs (tableau vide au départ)
- L'année de fondation

**Constructeur :**
- Doit initialiser l'équipe avec ses informations de base
- La liste de joueurs doit être vide au départ
- Paramètres : identifiant, nom, ville, entraîneur, année de fondation

**Méthodes requises :**
- Une méthode pour ajouter un joueur à l'équipe
- Une méthode pour retirer un joueur de l'équipe (par son numéro de joueur)
- Une méthode pour retourner le nombre total de joueurs dans l'équipe
- Une méthode pour afficher tous les joueurs de l'équipe avec leurs informations
- Une méthode pour retourner les informations de l'équipe (nom, ville, entraîneur, nombre de joueurs)
- Une méthode pour vérifier si un joueur existe dans l'équipe (par son numéro)
- Une méthode pour compter le nombre de joueurs par position

**Règles de visibilité :**
- Les propriétés doivent être `private`
- Les méthodes doivent être `public`
- Utilisez des getters pour accéder aux propriétés

### Travail à faire

1. Créez le fichier `Equipe.php`
2. Importez la classe `Joueur` (utilisez `require` ou `require_once`)
3. Déclarez la classe et ses propriétés
4. Écrivez le constructeur
5. Implémentez toutes les méthodes requises
6. Testez votre classe en :
   - Créant une instance d'équipe
   - Créant plusieurs joueurs
   - Ajoutant les joueurs à l'équipe
   - Affichant l'équipe et ses informations
   - Testant la suppression d'un joueur
   - Affichant le nombre de joueurs par position

   ## 📋 Exercice 3 : La classe Match

### Énoncé

Créez une classe `Match` pour représenter un match de football.

**Propriétés requises :**
- Un identifiant unique du match
- L'équipe à domicile (objet `Equipe`)
- L'équipe en déplacement (objet `Equipe`)
- La date du match (au format texte, par exemple "2024-03-15")
- Le lieu du match (stade)
- Les buts marqués par l'équipe à domicile
- Les buts marqués par l'équipe en déplacement
- Le statut du match ("À venir", "En cours", "Terminé")

**Constructeur :**
- Initialise tous les paramètres
- Le score commence à 0-0
- Le statut par défaut est "À venir"
- Paramètres : identifiant, équipe domicile, équipe déplacement, date, lieu

**Méthodes requises :**
- Une méthode pour mettre à jour le score (prend en paramètre l'équipe qui a marqué)
- Une méthode pour changer le statut du match
- Une méthode pour retourner le résultat du match (par exemple : "Lyon 3 - 2 Monaco")
- Une méthode pour déterminer l'équipe gagnante (ou "Match nul" s'il y a égalité)
- Une méthode pour afficher les informations du match de manière formatée
- Une méthode pour calculer le nombre total de buts du match

**Règles de visibilité :**
- Les propriétés doivent être `private`
- Les méthodes doivent être `public`

### Travail à faire

1. Créez le fichier `Match.php`
2. Importez les classes `Equipe` et `Joueur`
3. Déclarez la classe et ses propriétés
4. Écrivez le constructeur
5. Implémentez toutes les méthodes requises
6. Testez votre classe en :
   - Créant deux équipes avec plusieurs joueurs chacune
   - Créant une instance de match
   - Simulant l'ajout de buts au match
   - Affichant le résultat final
   - Affichant l'équipe gagnante

## 🎯 Exercice 4 : Mise en pratique complète

### Travail à faire

Créez un fichier `index.php` qui servira de point d'entrée à votre application. Ce fichier doit :

1. Importer les trois classes (`Joueur`, `Equipe`, `Match`)
2. Créer deux équipes de football complètes :
   - Équipe 1 : 5 joueurs minimum, avec différentes positions
   - Équipe 2 : 5 joueurs minimum, avec différentes positions
3. Créer un match entre ces deux équipes
4. Simuler le match :
   - Ajouter plusieurs buts au fur et à mesure
   - Changer le statut du match
   - Afficher les informations du match après chaque but
5. Afficher le résumé final du match avec :
   - Le score final
   - L'équipe gagnante
   - Les informations des deux équipes
   - La liste des joueurs de chaque équipe

---

## Concepts à comprendre pour le pattern MVC

En complétant cet exercice, vous avez manipulé :

- **Model (Modèle)** : Vos classes `Joueur`, `Equipe` et `Match` représentent les données métier
- **Logique métier** : Les méthodes de ces classes contiennent la logique de votre application
- **Séparation des responsabilités** : Chaque classe a une responsabilité claire

Pour aller vers le **pattern MVC**, vous allez bientôt ajouter :

- **Vue (View)** : Un fichier HTML/CSS pour afficher les données
- **Contrôleur (Controller)** : Un fichier PHP qui gère les interactions entre les modèles et les vues
- **Routeur** : Un mécanisme pour diriger les requêtes vers les bonnes actions

---

## Points importants à retenir

| Concept | Définition | Exemple |
|---------|-----------|---------|
| **Classe** | Un moule pour créer des objets | `class Joueur { }` |
| **Propriété** | Une variable au sein d'une classe | `private $nom;` |
| **Constructeur** | Méthode appelée lors de la création d'un objet | `public function __construct($nom)` |
| **Méthode** | Une fonction au sein d'une classe | `public function getNom()` |
| **Visibilité** | Définit qui peut accéder (public, private, protected) | `private $nom;` |
| **Objet** | Une instance d'une classe | `$joueur = new Joueur(...);` |
| **Getter** | Méthode pour lire une propriété privée | `public function getNom() { return $this->nom; }` |

---

## Astuces de développement

- Utilisez `$this` pour accéder aux propriétés et méthodes de la classe courante
- N'oubliez pas `new` pour créer une instance
- Utilisez `require_once` pour importer vos classes (et éviter les doublons)
- Testez progressivement : écrivez une classe, testez-la, puis passez à la suivante
- Commentez votre code pour expliquer vos choix
- Utilisez des noms de variables et méthodes explicites

---

