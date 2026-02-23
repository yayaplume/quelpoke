<img src="https://raw.githubusercontent.com/PokeAPI/media/master/logo/pokeapi.svg?sanitize=true" width="400" alt="PokeAPI">

# QuelPoke

### Service rendu
Application web (serveur Go) qui génère un Pokémon à partir d'un texte saisi,
via l'API [pokeapi.co](https://pokeapi.co).

### Fonctionnement global

Le texte saisi est hashé (SHA1), ce qui génère un ID Pokémon fixe (1-151).
L'app interroge ensuite PokeAPI pour récupérer le nom et affiche le résultat.

### Comment faire fonctionner l'appli?

Prérequis : Go 1.22+ installé.

```
git clone <repo> && cd quelpoke
go mod tidy  # Télécharge dépendances
go run main.go  # Lance sur http://localhost:8080

```

### Test
Dans un navigateur:
http://localhost:8080
​