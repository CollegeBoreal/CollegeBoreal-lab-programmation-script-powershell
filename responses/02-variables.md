## Utilisation de Variables

On va modifier notre script en donnant aux paramètres des types, on en déduit donc que ce sont des variables.

- [ ] Devant nos variables rajoutons les types comme ceci

```
[String]$personneNom = "Alice"
[Int]$personneAge = 35
```

- [ ] Aussi, nous allons évoquer quelques concepts qui existe dans des languages de programmation. La notion de `Pattern Matching` qui lie une variable à plusieurs variables. Si un `pattern` est trouvé il faut sortir avec l'instruction `break`

Place le code ci dessous à la fin du script

```powershell
# Test sur l'age de la personne
switch ($personneAge) {
    {$_ -le 25} {Write-Host 'en pleine jeunesse'; break }
    {$_ -le 35} {Write-Host 'en pleine force vive'; break }
    {$_ -le 45} {Write-Host 'en pleine maturité'; break }
    Default {Write-Host 'en pleine serénité'}
}
```

Maintenant fais tourner ton code et mets la *dernière* phrase affichée que tu as trouvé dans le commentaire et faisons rouler ce tutoriel!
