Continuons maintenant avec l'autre script qui ca nou permettre de créer un fonction en PowerShell.

Ouvre le script `b000000000-fonction.ps1`

Tu y trouveras la definition de la fonction ainsi que son appel juste en dessous de la definition

```powershell
# Definition de la fonction
function Stagiaire {

}

# Appel de la fonction
Stagiaire
```

- [ ] Ajoute des paramètres à la fonction. Dans le corps de la fonction rajoute le code suivant en respectant l'indentation:

```python
    param (
        [String]$personneNom,
        [Int]$personneAge
    )
```

- [ ] Affichage, toujours dans le corps de la fonction rajoute le code suivant en respectant l'indentation:

```
    # message de bienvenue 
    "Bonjour {0} ! Tu as {1} ans." -F $personneNom, $personneAge
```

Comme tu peux le remarquer, le formattage utilise de d'affichage à l'aide de variables positionnelles. `{0}` indiquant la position de la variable `$personneNom` et `{1}` indiquant la position de la variable `$personneAge`


- [ ] À l'appel de la fonction, rajoute la première ville du tableau `$villes` que l'on a vu dans l'exercice précédent en premier paramètre (remplace `--VILLE--`) ainsi que l'age d'Alice en deuxième paramètre (remplace `--AGE--`) .

```
# Appel de la fonction
Stagiaire --VILLE-- --AGE--
```

- [ ] Exécute ton code et ajoute en commentaire l'impression que tu as obtenu. On passera ensuite au code suivant.
