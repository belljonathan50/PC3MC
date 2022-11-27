# PC3MC
Dans PC3MC/puredata/sounds, créer 4 ou 5 fichiers son chacun avec des index différents selon les auteurs
en mono .wav 44100, moins longs que 4 min 30 = 25MB


son1.wav son2.wav son3.wav son4.wav son5.wav jonathan
son6.wav son7.wav son8.wav son9.wav matheo
son10.wav son11.wav son12.wav son13.wav son14.wav elise
son15.wav son16.wav son17.wav son18.wav son19.wav theo...

Copier ces fichiers dans PC3MC/sounds (vide par défaut, limitation github...)

Dans PC3MC/puredata/onsets, créer les fichers correspondants:

son1.txt son2.txt son3.txt son4.txt son5.txt jonathan
son6.txt son7.txt son8.txt son9.txt matheo
son10.txt son11.txt son12.txt son13.txt son14.txt elise
son15.txt son16.txt son17.txt son18.txt son19.txt theo...


rajouter à la fin des fichiers d'onset (de type "onsets/son1.txt")
les metadonnées suivantes:
- un entier déterminant l'index du fichier son
- nombre de slices (number of slices:)
- source du matériau (source: modalys)
- auteur (Théo)
- des groupes d'index de slices en prévision de l'écriture en antescofo

soit pour les 5 premiers sons:

1 222 glockenspiel-flute-piano feldman
2 151 electronics romina
3 232 harp baker
4 113 cordes samuel-poirot
5 45 plaque samuel-poirot 

Les fichiers d'onset ont le même nom que le fichier son correspondant de type "sounds/son1.wav")

limiter la tailler des fichier son à 25MB pour communication fluide sur github
