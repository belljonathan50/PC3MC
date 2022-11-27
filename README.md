# PC3MC

# modèle physique, classification de timbre,  Synthèse concaténative

Après collecte de sons dans derailer ou modalys, dans puredata/sounds, créer 4 ou 5 fichiers son chacun avec des index différents selon les auteurs, en mono .wav 44100


son1.wav son2.wav son3.wav son4.wav son5.wav jonathan

son6.wav son7.wav son8.wav son9.wav matheo

son10.wav son11.wav son12.wav son13.wav son14.wav elise

son15.wav son16.wav son17.wav son18.wav son19.wav theo...

Dans puredata/onsets, créer les fichers correspondants, à partir des dates "vertes" dans classificationduo.maxpat :

son1.txt son2.txt son3.txt son4.txt son5.txt jonathan

son6.txt son7.txt son8.txt son9.txt matheo

son10.txt son11.txt son12.txt son13.txt son14.txt elise

son15.txt son16.txt son17.txt son18.txt son19.txt theo...

ces fichiers contiennent jusqu'à 250 dates


rajouter à la fin des fichiers d'onset (de type "onsets/son1.txt")
les metadonnées suivantes:

- "son" + un entier déterminant l'index du fichier son (exemple: "file son1")

- le nombre de slices pour ce fichier son (NumItems 222)

- minslicelength nombre de slices (param minslicelength pour obtenir cette analyse exemple "minslicelength 80")

- threshold (sensibilité du paramètre threshold exemple "threshold 0.3")

- source du matériau (exemple "source: modalys")
- auteur ("auteur Théo")

- des groupes d'index de slices qui s'enchaînent bien (en prévision de la composition pour acousmonium mobile) (exemple "enchainements: 32 43 54 67 ")

soit pour le premier son (à la fin du fichier):

file: son1.wav NumItems: 222 minslicelength:  222 threshold: 0.252 source: glockenspiel-flute-piano auteur: feldman enchainements: 32 43 54 67 - 45 49 40 48
https://raw.githubusercontent.com/belljonathan50/PC3MC/main/puredata/onsets/son1.txt

et pour les suivants:

file: son2.wav minslicelength: 151 minslicelength: 80 source: electronics romina  enchainements: 132 123 34 67 - 35 29 10 148...



Les fichiers d'onset ont le même nom que le fichier son correspondant de type "sounds/son1.wav")

# Composition via antesofo sur raspberry
antescofo "maître" (antescofo-compo/cuelist.maxpat), envoie des déclenchements aux patchs clients (puredata:patchrasp.pd)

dans "antescofo-compo", modifier MyName.asco.txt, par exemple:
MyName.asco.txt -> TheoYepez.asco.txt
