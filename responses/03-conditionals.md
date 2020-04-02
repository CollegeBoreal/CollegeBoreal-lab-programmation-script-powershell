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



- [ ] Exécute ton code et ajoute en commentaire l'impression que tu as obtenu. On passera ensuite au code suivant.
