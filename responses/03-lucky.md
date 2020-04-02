{{ personne }} :tada: :tada: :tada: 

C'est ce que l'on appelle un parcours sans faute.

## Tracer la visite d'une personne

Il nous reste maintenant à rajouter un bout de code servant à débugger le script.

- [ ] Rajoutons un décorateur `[CmdletBinding()]`  aux paramètres d'entrées

```powershell
    [CmdletBinding()]
    param (
        [String]$personneNom,
        [Int]$personneAge
    )
```

- [ ] Ensuite entourons l'affichage des informations de la personne avec un `début`, un `traitement` (process) et une `fin`, comme ceci:

```powershell
    BEGIN {Write-Verbose "Début du script"}
    PROCESS { "Bonjour {0} ! Tu as {1} ans." -F $personneNom, $personneAge }
    END {Write-Verbose "Fin du script"}
```

Il faut remarquer l'affichage à l'écran est maintenant obtenue avec l'instruction `Write-Verbose` qui nous permettra de faire du déboggage en l'affichant ou pas en rajoutant le paramètre `-Verbose` à l'appel de la fonction

:bulb: Si tu as bien suivi le code, tu devrais trouver la fonction `Stagiaire` comme ceci si tu tapes la commande `git diff` dans ton terminal

```python
 # Definition de la fonction
 function Stagiaire {
+    [CmdletBinding()]
     param (
         [String]$personneNom,
         [Int]$personneAge
     )
     # message de bienvenue 
-    "Bonjour {0} ! Tu as {1} ans." -F $personneNom, $personneAge
+    BEGIN {Write-Verbose "Début du script"}
+    PROCESS { "Bonjour {0} ! Tu as {1} ans." -F $personneNom, $personneAge }
+    END {Write-Verbose "Fin du script"}
 
 }
 ```

:star:  `git diff` représente la différence entre le code en train d'ètre modifié et le code soumit sur GitHub

* Les lignes précédées d'un signe `+` sont les lignes ajoutées

* Les lignes précédées d'un signe `-` sont les lignes supprimées

- [ ]  Éxécute ton programme pour tester ton nouveau code mais avant rajoute l'appel de fonction suivant à la fin de ton script avant de l'éxécuter

```
Stagiaire "Pascal Siakam" 26  -verbose
```


**Soumet ton code** vers GitHub pour continuer:
```
git add b000000000-fonction.ps1
git commit -m "Tutoriel complété"
git push
```
