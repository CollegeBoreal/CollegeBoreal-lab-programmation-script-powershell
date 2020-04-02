Chèr.e {{ id }}, il est temps de faire de la programmation!

- [ ] Changer l'auteur du programme Python dans le script `b000000000-structure.ps1`

```powershell
<#
.SYNOPSIS
    Ce script est une laboratoire Powershell

.DESCRIPTION
    Ce script est utilisé pour le laboratoire de programmation en Powershell.

.NOTES
    Author: CollegeBoreal
    Derniere mise à jour: yyyy-mm-dd

#>
```

Modifie le script Powershell avec l'éditeur de ton choix et changer l'auteur `CollegeBoreal` avec ton :id: Github

- [ ] Exécuter le script PowerShell

Voyons voir le script Powershell, on peut y voir une commande `Write-Host` qui imprime du texte à la console du terminal:

```powershell
Write-Host "Bonjour Monde"
```

- [ ] Avant le code `Write-Host "Bonjour Monde"`, on va insérer des parametres pour rendre l'impression plus dynamique.

```powershell
$personneNom = "Alice"
$personneAge = 35
```

- [ ] On va ensuite remplacer l'impression de "Bonjour Monde" avec une version avec parametres:

```powershell
Write-Host "Bonjour $personneNom, tu as $personneAge ans. "
```

- [ ] Fais tourner ton programme dans ton terminal

Pour éxécuter le script PowerShell taper `b000000000-structure.ps1` dans le terminal. Le script PowerShell doit se trouver dans le même répertoire ou l'on se trouve.

* Sous Windows:

```
PS > .\b000000000-structure.ps1
```

* Sous pwsh (Sous :apple:)

```
% ./b000000000-structure.ps1
```


Après l'éxécution, sur votre terminal s'affichera: "Bonjour Alice, tu as 35 ans.". Nous ferons mieux dans quelques instants mais pour l'instant, il faut soumettre le code vers GitHub. 


- [ ] Soumettre les modifications

Pour chaque changement de fichiers dans ton référentiel, il faut  `ajouter` et `signer` le fichier qui te permet de formuler un message detailant ce que tu as changé. Ensuite tu peux `soumettre` une version mise à jour, en même temps que tes commentaires, vers GitHub. 

:round_pushpin: Faisons ces trois étapes:

1. Ajouter dans Git: `git add b000000000-structure.ps1`
2. Signer dans Git: `git commit -m "Embellir son bonjour"`
3. Soumettre à Git: `git push`
