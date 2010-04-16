#=================================================================================================================#
#============================================= Un peu d'histoire... ==============================================#

Il était une fois, dans une galaxie lontaine, très lointaine... (mais furieusement ressemblante au système dans 
lequel nous vivons)

....................
blabla, Gordon's Story
....................


#=================================================================================================================#
#================================== Composition et fonctionnement de la scène ====================================#

_________________________
! Précisions techniques !
------------------------- 
Il semblerait que certains affichages se fassent différement selon les visualiseurs VRML employés.
Pour un divertissement de qualité maximale, nous vous recommandons d'utiliser Cortona Viewer.

Si la scène est trop ralentie et que les déplacements sont saccadés, il peut être approprié de modifier la quantité
d'astéroïdes présents dans la scène. Pour cela, ajustez les champs "copies" aux alentours des lignes 225 et 254
dans le fichier "system.wrl".

_______________________

La scène se visite en deux temps. L'utilisateur l'aborde d'abord à une petite échelle, qu'il doit considérer a
priori comme étant tout l'espace visitable ; il s'agit de la base entourée de montagnes. Ensuite, il peut, à sa 
grande surprise, envisager de s'envoller pour s'élever davantage et progresser vers des dimensions toutes autres
(essentiellement à l'aide des points de vue).

___________________
I-La base terrestre
-------------------


____________________
II-Le système Exodus
--------------------

Il s'agit d'un système planétaire proche de notre système solaire (on y trouve en effet une seconde Terre !), aux 
comportements identiques modulo quelques libertés prises.

La scène est accompagnée d'une musique d'ambiance extraite du jeu de rôle space opera qu'est Mass Effect.

	_________________
	II-1) Composition
		a) Corps célestes

Le système Exodus est composé de cinq planètes gravitant autour de l'astre en fin de vie Exodus, avec une ceinture
d'astéroïdes. Dans l'ordre croissant d'éloignement à Exodus :

	-planète Terre (Earth), avec sa lune ; c'est ici qu'est positionnée la base détaillée ci-dessus
	-ceinture d'astéroides (modèle Styx) ; des ceintaines d'astéroïdes en rotation rapide, isolant la Terre
du reste du système.
	-Acheron, planète massive à la surface brunâtre. Intéressante à plus d'un points pour ses ressources
minérales.
	-Theseus, planète moyenne, à anneaux elliptiques, à la surface aride et quasi désertique. C'est un endroit
idéal pour y dissimuler des activités dissidentes.
	-Erebus, petite planète verte, à l'atmosphère viciée, a priori rendant toute vie organique impossible. Des
sondes ayant cependant enregistré des signaux sonores étranges à sa proximité font suspecter qu'une civilisation extraterrestre intelligente s'y est probablement développée (serait-ils responsables du plan de révolution
inhabituel et non naturel observé pour cette planète ?). 
	-Antaeus, petite planète à la surface bleuté par les océans qui la recouvrent totalement. Intérêt mineur.

Chaque planète posséde sa propre atmosphère.

Exodus baigne tout le système d'un bruit continu et à très basses fréquences, si propre à ce type d'astre 
rayonnant et en pleine activité nucléaire.

		b) Vaisseaux

On y trouve deux types de vaisseaux :
-les flottes impériales et rebelles qui semblent se chasser indéfiniment. 
-un vaisseau extraterrestre (OVNI) circulaire à l'origine encore inconnue, mais suspecté provenir d'Erebus. 
Une entité supérieure indéterminée semble provoquer des déplacements sans le moindre schéma logique.

Curieusement, malgré le vide constaté de l'espace, les habitués aux voyages interplanétaires témoignent du bruit
que peuvent faire certains de ces vaisseaux lorsque l'on se trouve à proximité de ces derniers. Les rebelles semblent être parvenus toutefois à trouver un mode de déplacement furtif et non sonorisé, mais à l'origine d'une
étrange projection de lumière.

	_________________
	II-2) Interaction

		a) Déplacements

Au vu de l'échelle, il est préférable d'utiliser les points de vue (clic droit, "Viewpoints") pour se déplacer
d'un objet à l'autre dans la scène. Chaque objet a à cet effet au moins un point de vue qui lui est propre, et 
choisi de telle sorte que l'on ait par la même occasion un aperçu du reste du système.
Sinon, le mode de déplacement "Examine" (icône en forme d'oeil en bas à gauche) est approprié, ainsi que le mode
"Fly" (icône papillon) dans une moindre mesure.

		b) Interaction avec le vaisseau (OVNI)

D'abord, pour apprécier au mieux cette fonctionnalité, il est recommandé de choisir le point de vue "Exodus
 Cluster" ou bien "God's eye view" pour avoir une vue d'ensemble et profiter de déplacements facilités.

Sur le système se remarque un plan circulaire transparent (si ce n'est pas le cas, modifier le champ de 
transparence, autour de la ligne 650 du fichier "system.wrl") cliquable. En maintenant dessus un clic gauche, il
est possible de faire se déplacer une cible carrée verte, vers laquelle se dirigera systématiquement et
automatiquement le vaisseau-OVNI circulaire gris.

Sa particularité est qu'il évitera toutes les planètes en déplacement et l'astre central (Exodus) sur son passage :
aucun de ces corps célestes n'est traversable par cet objet.

		c) Animations

Les animations automatiques sont de trois sortes :

-chaque planète tourne sur elle-même et autour de l'étoile Exodus, avec une période de révolution fonction de sa
distance à cet astre. La lune tourne autour de la Terre.

-l'astre central Exodus simule un rayonnement et une coloration dynamique.

-Des flottes de trois vaisseaux de déplacent périodiquement de la planète Acheron à la planète Theseus (planète à
anneaux), pour y attérir et y décoller (cela se manifeste visuellement par leur arrêt au-dessus de ces planètes
suivi de leur disparition momentanée). 
Ces vaisseaux se meuvent en gravitant en "spirale" autour d'Exodus pour rejoindre sans encombre leur destination.
Ils y parviendront quelle que soit la position et l'orientation de la planète à atteindre à tout moment
(animations non totalement précalculés, mais adaptées au contexte), et se déplacent aussi verticalement afin de
 s'adapter au rayon de la planète en question (pour se rapprocher de la surface). 


#=================================================================================================================#
#=================================================== Crédits =====================================================#

Projet réalisé par Yohann Rubinsztejn et Michaël Ludmann dans le cadre de l'option robotique et réalité virtuelle 
de 2ème année suivie à l'ENSIIE en 2010.

Enseignement encadré par M. Guillaume Bouyer.

Note : les fichiers "destroyer.wrl" et "wing.wrl" ne sont pas de notre fait. Pour retrouver leurs sources, se
réferer aux en-têtes de ces fichiers.