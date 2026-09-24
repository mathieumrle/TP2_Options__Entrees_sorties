TP2 Options et Entrée/Sorties

Partie I : Compte-rendu
Votre compte-rendu doit être rédigé en Markdown, en utilisant les balises adaptées (titres,
listes, mise en forme du code, etc.) et en veillant à la propreté du texte brut. Indiquez
simplement le numéro de la question avant chaque réponse. Les images ne sont autorisées
que si elles apportent une réelle plus-value à la compréhension. Enfin, déposez votre fichier
sur la plateforme Eléa avant la fin de la séance, dans la zone de dépôt dédiée avec votre
fichier markdown ou compressé (zip) en le nommant de la sorte : NOM_TP2.format.

Partie II : Les options
Les questions suivantes nécessitent la lecture du manuel avec la commande man. Essayez
de prendre l’habitude de trouver par vous-même les informations dont vous avez besoin.
En utilisant la VM SYS-TP-D13 du TP1 et en reprenant l’arborescence du TP1 faire les
questions suivantes :
1. Par défaut cp ne copie que des fichiers. L’option-r permet de forcer cp à copier
les répertoires et sous-répertoires du répertoire qui lui est donné en argument (cela
s’appelle une copie récursive). Utiliser la commande cp-r sur le répertoire Cours
à destination du répertoire Perso. Quelle commande avez-vous utilisé?
2. Créer une copie de readme.md appelée .texte.txt (le point devant est voulu) dans
votre répertoire personnel (Perso). Quelle commande avez-vous utilisé?
3. Faire la commande ls dans le répertoire Perso. Que remarquez-vous?
4. Trouver l’option de ls qui permet d’afficher les fichiers cachés. Quelle est l’option?
5. Par défaut, le résultat de la commande ls est un peu aride. Une option permet de
colorer l’affichage pour repérer plus rapidement le type de fichiers présents dans un
répertoire. Quelle est cette option de ls?
6. Quelle est l’option de rm permettant d’effacer récursivement un répertoire (c’est à
dire en descendant dans les sous-répertoires)? Appliquer-la sur le répertoire Cours
qui est situé dans Perso.
7. Par défaut, rm ne demande pas de confirmation lorsque vous tentez de supprimer un
fichier. Ceci peut se révéler assez dangereux. Trouver et donner l’option qui permet
de demander la confirmation de la suppression.

Partie III : Les entrées/sorties
Pour cette partie, créer un nouveau répertoire IO et se placer dedans.
8. Utiliser la commande echo pour afficher le texte "Bonjour, BTS SIO!" et rediriger
cette sortie dans un fichier nommé bonjour.txt. Afficher ensuite le contenu de
bonjour.txt pour vérifier la redirection. Quelle commande avez-vous utilisée?
9. Utiliser l’opérateur de redirection » pour ajouter la ligne "L’apprentissage de Linux
est essentiel." à la fin du fichier bonjour.txt. Vérifier le contenu du fichier. Que
se passe-t-il si vous utilisez > au lieu de »?
10. Créer un fichier nommé exemple.txt et écrire au moins 10 lignes. Utiliser la com
mande sort pour trier le contenu du fichier exemple.txt. Rediriger l’entrée de
cette commande avec <. Quelle est la commande complète que vous avez utilisée?
Affichez le résultat trié dans le terminal.
11. Utiliser grep pour trouver toutes les lignes dans exemple.txt contenant le mot
"Linux", puis utilisez un pipe (|) pour trier ces lignes par ordre alphabétique.
Quelle est la commande complète que vous avez utilisée, et quel est le résultat?
12. Essayer de lister le contenu d’un répertoire inexistant (ls /dossier_inexistant).
Rediriger le message d’erreur vers un fichier nommé erreurs.txt. Quelle est la
commande complète et que contient le fichier erreurs.txt après l’exécution?

Partie IV : Les métacaractères
Il existe un certain nombre de symboles spéciaux appelés métacaractères ou wildcards. Ils
permettent de désigner plusieurs fichiers à la fois. Il en existe plusieurs, mais les principaux
sont : * : dans un nom de fichier, représente n’importe quelle suite de symboles. ? :
représente exactement un symbole quelconque.
Ainsi, écrire : tp?.ps désigne tp1.ps ou tpi.ps mais pas tp-sio.ps.
mai* désigne maison, mais, mairie mais pas semaine.
13. Afficher la liste de tous les fichiers dans le répertoire /usr/bin dont le nom com
mence par k et contient exactement 7 caractères.
14. Afficherlaliste de tous les fichiers dont l’extension est so dans le répertoire /usr/lib
(note culturelle : ces fichiers sont des bibliothèques)