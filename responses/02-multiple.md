Tu as entré {{ taille }} , j'ai trouvé `en pleine force vive` . Cela n'a pas trop d'importance pour l'instant, continuons!.

- [ ] Structure de donnée - Tableau

Jouons encore avec une variable, cette fois ci un tableau. À la fin du script `b000000000-structure.ps1` , rajoute ce code:

```powershell
$villes = "Toronto","Mississauga","Scarborough","Brampton"
```

- [ ] Structure de contrôle

Nous avons tous vu ce code de type `programmation impérative` qui fait tourner le monde: La boucle impérative. Continue en entrant ce code ainsi que le commentaire qui va avec à la fin du script. Un commentaire sur une seule ligne commence avec le caractère `#`

```powershell
for ($i = 0; $i -le $villes.Count; $i = $i + 1) {
    $villes[$i]
}

#Clear-Host

```

Fais tourner ton script dans ton terminal.

- [ ] Modulons

Comme tu as pu le remarquer le tableau `$villes` à une variable publique `Count` qui nous donne la taille du tableau. Dan notre cas, on veux savoir si cette taille est paire. Pour le savoir on va utilise l'opérateur Modulo `%` et si la taille est impaire (le reste de la division), on obtient un `1`

Au lieu d'utiliser l'instruction `Write-Host` pour afficher, on prendra le formattage suivant qui utilise des variables positionnelles (plus de contenu juste un peu plus tard): 

:warning: Pour permettre l'affichage du résultat uniquement, enleve le commentaire `#` de l'instruction `Clear-Host` qui permet de nettoyer tout l'écran et rajoute le code suivant.

```
"{0}" -F ($villes.Count % 2)
```

- [ ] Refais tourner ton script dans ton terminal

:bulb: Mets l'affichage imprimé par le script dans le message de ta signature `commit` à la soumission de ton programme.


**Soumets ton code** vers GitHub pour continuer:
```
git add b000000000-structure.ps1
git commit --message "La reste du Modulo est <remplace ICI>"
git push
```
