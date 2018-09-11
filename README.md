# DAC Project

##Authors:
-K�vin BEDIN
-Quentin DUCASSE
-Steve Carlson KASSE MIKUI
-Guillaume LE BOUCHER
-Luc LONGIN

##Mise en place Github
Obtenir une copie du projet sur votre compte github : ==fork==
Cr�er une copie locale du projet git sur votre ordinateur :
[[[language=bash
$ git clone https://github.com/NomDeCompte/Projet-DAC
]]]

D�s que vous modifiez un �l�ment de votre dossier git, une ==working copy== est cr��e. Pour mettre � jour votre copie locale :
Ajout � la pile de ==commit== 
[[[language=bash
$ git add nomDuFichier
]]]
Puis commit pour modifier les fichiers locaux :
[[[language=bash
$ git commit -m 'Message du commit'
]]]
La modification n'op�re que sur votre copie locale, ni le dossier github de votre compte ni celui du compte d'o� provient le ==fork== a �t� modifi�.

Pour modifier votre copie virtuelle :
[[[language=bash
$ git push
]]]

Maintenant, pour mettre � jour votre copie virtuelle et locale en cas de modification du dossier initial (celui que vous avez ==fork==) il faut utiliser un ==remote==. Le ==remote== est un pointeur vers un le dossier git voulu :
Mise en place du ==remote== appel� ==upstream== par :
[[[language=bash
$ git remote add upstream https://github.com/bedinke/Projet-DAC
]]]
Mise � jour de votre dossier local et virtuel :
[[[language=bash
$ git fetch upstream
$ git checkout master
$ git merge upstream/master
]]]