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

- [ ] Ajoute des paramètres à la fonction, Dans le corps de la contion rajoute le code suivant en respectant l'indentation:

```python
    param (
        [String]$personneNom,
        [Int]$personneAge
    )
```

La traversée de l'abre est presqu'inutile car nous l'avons traversé dans son entier sans avoir trouvé l'élu. Nous devons donc revenir sur nos pas et :

* insérer la fonction définie plus tôt `personne_elue()`

* trouver au plus vite l'élu(e) 

* et sortir de l'arbre dés que l'on peut. 


- [ ] L'insertion de ce nouvel élément se fera juste à la sortie du bus `popleft()` et avant que la personne `rameute` ses amis `search_queue += eleves[personne]`.

```python
      if personne_elue(personne):
         print(personne + " a le fameux Mac")
         return True
```

:bulb: Le code final de notre algorithme devrait ressembler à ceci, vérifie que le code ci dessous correspond à celui de ton programme:

```python
   while search_queue:
      personne = search_queue.popleft()
      if personne_elue(personne):
         print(personne + " a le fameux Mac")
         return True
      search_queue += eleves[personne]
```

- [ ] Exécute ton code et ajoute en commentaire l'impression que tu as obtenu. On passera ensuite au code suivant.
