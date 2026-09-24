# TP2 – Options et Entrées/Sorties

## Partie II : Les options

**1.**
```bash
cp -r Cours Perso
```

**2.**
```bash
cp Perso/readme.md Perso/.texte.txt
```

**3.**
```bash
ls Perso
```
On voit `Cours` et `readme.md`, mais pas `.texte.txt` : les fichiers dont le nom commence par un point sont cachés.

**4.**
```bash
ls -a Perso
```
(ou `ls --all`)

**5.**
```bash
ls --color Perso
```
(ou `ls --color=auto`)

**6.**
```bash
rm -r Perso/Cours
```

**7.**
```bash
rm -i
```

## Partie III : Les entrées/sorties

```bash
mkdir IO
cd IO
```

**8.**
```bash
echo "Bonjour, BTS SIO !" > bonjour.txt
cat bonjour.txt
```

**9.**
```bash
echo "L'apprentissage de Linux est essentiel." >> bonjour.txt
cat bonjour.txt
```
Avec `>` au lieu de `>>`, le fichier est écrasé : l'ancien contenu est perdu.

**10.**
```bash
printf "pomme\nLinux est libre\nzebre\nbanane\nDebian\nLinux est stable\ncarotte\nSIO\nreseau\nLinux en BTS\n" > exemple.txt
sort < exemple.txt
```

**11.**
```bash
grep "Linux" exemple.txt | sort
```
Résultat :
```
Linux en BTS
Linux est libre
Linux est stable
```

**12.**
```bash
ls /dossier_inexistant 2> erreurs.txt
cat erreurs.txt
```
Contenu de `erreurs.txt` :
```
ls: impossible d'accéder à '/dossier_inexistant': Aucun fichier ou dossier de ce type
```

## Partie IV : Les métacaractères

**13.**
```bash
ls /usr/bin/k??????
```

**14.**
```bash
ls /usr/lib/*.so
```
