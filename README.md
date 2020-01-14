# Programmation répartie

## Documents : tous les fichiers sont accessibles dans le dossier [`M412`](M412) ci-dessus.

## DS : une feuille manuscrite recto-verso A4 de notes personnelles autorisée.

## Supports

Supports du module de DUT INFO TDFT02 TDFM412 2019-2020 
Ces fichiers sont mis à jour tout au long du semestre.

 - [x] Séance 1 : TD_THREADS
 - [ ] Séance 2 : suite TD_THREADS
 - [ ] Séance 3 : Framework Executor
 - [ ] Séance 4 : Sockets
 - [ ] Séance 5 : Cours RMI et suite TD sockets / servers (sous réserves)
 - [ ] Séance 6 : TD échanges de messages multi hosts
 - [ ] Séance 7 : début de correction et suite

Pour une meilleure lecture, téléchargez et visualisez les fichiers pdf sur votre disque local.

| Cours et énoncés de TD/TP |
| :---         |
| [Cours d'introduction sur la programmation répartie](M412/Cours_1_M412_INTRO.pdf "Cours d'introduction sur la programmation répartie") |
| [Cours 1 sur la concurrence et les threads Java](M412/Cours_1_M412_CONCURRENCE.pdf "Cours 1 sur la concurrence et les threads Java") |
| [TD 1 sur les threads Java](M412/TD_THREADS/td_1_threads_java.pdf "TD 1 sur les threads Java") |

| Liens utiles |
| :---      
| [Java tutorial: concurrency](https://docs.oracle.com/javase/tutorial/essential/concurrency/index.html "tutoriel oracle")|
| [Java tutorial: custom networking](https://docs.oracle.com/javase/tutorial/networking/TOC.html "tutoriel oracle")|


## Attention :heavy_exclamation_mark:
Ce serveur web n'est pas forcément toujours disponible en dehors des heures de TP, pensez à synchroniser les fichiers sur votre poste de travail.

### Conseil pour les TD, utilisation basique de git

#### Configuration
Configurez votre environnement (fichier `.gitconfig` à la racine de votre compte)

Exemple sous Windows (fichier `C:\Users\login`):
```
[http]
	sslVerify = false

[user]
	name = Prenom NOM
	email = Prenom.NOM@unice.fr

[gui]
	encoding = utf-8

[core]
	autocrlf = false

[credential]
	helper = wincred
```

Exemple sous Linux (fichier `$HOME/.gitconfig`):
```
[user]
	name = Prenom NOM
	email = Prenom.NOM@unice.fr

[core]
        autocrlf = false
        safecrlf = true
        editor = emacs

[alias]
        co = checkout
        ci = commit
        st = status
        br = branch
        hist = log --pretty=format:'%h %ad | %s%d [%an]' --graph --date=short
        type = cat-file -t
        dump = cat-file -p

[http]
        sslverify = false

[credential]
        helper = cache --timeout=3600

```

#### Première utilisation sur un poste local ou sur votre portable

Dans un terminal (clic droit et `Git Bash Here` sous Windows), on récupère d'abord son dépôt:

```
git clone https://github.com/uns-iut-info/G[1-4]_Prenom_NOM.git GITHUB
```

et aussi le dépôt contenant les fichiers de cours/TD/TP:

```
git clone https://github.com/uns-iut-info/doc-m412.git Cours_TD_M412
```

Ensuite vous travaillez dans vos dossiers / workspace habituels. À la
fin de la séance vous recopiez les fichiers réponse dans le dossier
GITHUB/M412/TD_NOM_DU_TD, puis vous mettez à jour votre dépôt distant.

```
cd GITHUB/
git add .
git commit -m "TD nom du td"
git push origin master
```

#### Utilisations suivantes

Si vous travaillez sur la même machine, allez successivement dans les
dossiers GITHUB et Cours_TD_M412, et mettez les à jour avec la
commande:

```
git pull
```

En fin de TD, procédez comme décrit ci-dessus pour la mise à jour du dépôt distant.

---

![Tamagotchi Hive](https://imgs.xkcd.com/comics/tamagotchi_hive.png "XKCD")
