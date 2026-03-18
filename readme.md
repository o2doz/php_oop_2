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
