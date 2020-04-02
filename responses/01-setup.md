  Bienvenue dans ce laboratoire qui te guidera à écrire un programme dans le language de script [PowerShell](https://docs.microsoft.com/fr-ca/powershell/scripting). Le programme se concentrera sur l'étude des structures des données de base ainsi que quelques structures controles les plus connues. Avant de commencer, nous allons nous assurer que l'environnement de développement est prêt. 

## :a: Installer PowerShell

:zero: Présence de Powershell

Ouvrir un terminal, sous Windows ouvrir `CMD`  et vérifier la version de Powershell avec la commande suivante

:round_pushpin: Windows `CMD`

```
C:\> powershell -Command "Get-Host | Select-Object Version"

Version
-------
5.1.17763.592
```

:round_pushpin: MacOS `bash` ou `zsh`

:warning: la commande s'écrit `pwsh` et non `powershell` 

```
% pwsh -Command "Get-Host | Select-Object Version" 

Version
-------
7.0.0
```

Si Powershell est installé, le résultat de la commande donnera une version. Cette version doit être superieure à `5.x.x`

:one: installer Python avec un `Package manager`

Si Python n'est pas installé, utiliser un gestionnaire de librairies.

:computer: Windows c'est installé par défaut

:apple: MacOS avec [HomeBrew](https://docs.brew.sh/Installation)

```
% brew cask install powershell
```

## :b: Installer [Git](https://git-scm.com/downloads)

:two: Présence de Git

Ouvrir un terminal et vérifier la version de Git avec la commande suivante

```
% git --version
```

Si le résultat donne un numéro de version. C'est parfait sinon

:four: installer Git avec un `Package manager`

Si Git n'est pas installé, utiliser un gestionnaire de librairies.

:computer: Windows avec [choco](https://chocolatey.org/install)

```
PS > choco install git.install
```

:apple: MacOS avec [HomeBrew](https://docs.brew.sh/Installation)

```
% brew install git
```

## :ab: Cloner le référentiel

Maintenant que nous avons Git, nous pouvons cloner le référentiel contenant block d'assemblage du code quer tu vas écrire. Dans un terminal tapes `git clone {{ repoUrl }}`, la version `SSH` est également recommandée

Dans le référentiel, il y a deux fichiers:

- `README.md`: un fichier `markdown` donnant des informations sur le laboratoire
- `b000000000-structure.ps1`: un script `PowerShell` contenant le code à construire pour les structures de données et controles
- `b000000000-fonction.ps1`: un autre script `PowerShell` contenant le code à construire pour les fonctions

Maintenant que tout est en place, nous pouvons commencer.

Laisses un commentaire avec ton *:id:* github pour continuer.
