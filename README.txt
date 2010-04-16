#=================================================================================================================#
#============================================= Un peu d'histoire... ==============================================#

Il �tait une fois, dans une galaxie lontaine, tr�s lointaine... (mais furieusement ressemblante au syst�me dans 
lequel nous vivons)

....................
blabla, Gordon's Story
....................


#=================================================================================================================#
#================================== Composition et fonctionnement de la sc�ne ====================================#

_________________________
! Pr�cisions techniques !
------------------------- 
Il semblerait que certains affichages se fassent diff�rement selon les visualiseurs VRML employ�s.
Pour un divertissement de qualit� maximale, nous vous recommandons d'utiliser Cortona Viewer.

Si la sc�ne est trop ralentie et que les d�placements sont saccad�s, il peut �tre appropri� de modifier la quantit�
d'ast�ro�des pr�sents dans la sc�ne. Pour cela, ajustez les champs "copies" aux alentours des lignes 225 et 254
dans le fichier "system.wrl".

_______________________

La sc�ne se visite en deux temps. L'utilisateur l'aborde d'abord � une petite �chelle, qu'il doit consid�rer a
priori comme �tant tout l'espace visitable ; il s'agit de la base entour�e de montagnes. Ensuite, il peut, � sa 
grande surprise, envisager de s'envoller pour s'�lever davantage et progresser vers des dimensions toutes autres
(essentiellement � l'aide des points de vue).

___________________
I-La base terrestre
-------------------


____________________
II-Le syst�me Exodus
--------------------

Il s'agit d'un syst�me plan�taire proche de notre syst�me solaire (on y trouve en effet une seconde Terre !), aux 
comportements identiques modulo quelques libert�s prises.

La sc�ne est accompagn�e d'une musique d'ambiance extraite du jeu de r�le space opera qu'est Mass Effect.

	_________________
	II-1) Composition
		a) Corps c�lestes

Le syst�me Exodus est compos� de cinq plan�tes gravitant autour de l'astre en fin de vie Exodus, avec une ceinture
d'ast�ro�des. Dans l'ordre croissant d'�loignement � Exodus :

	-plan�te Terre (Earth), avec sa lune ; c'est ici qu'est positionn�e la base d�taill�e ci-dessus
	-ceinture d'ast�roides (mod�le Styx) ; des ceintaines d'ast�ro�des en rotation rapide, isolant la Terre
du reste du syst�me.
	-Acheron, plan�te massive � la surface brun�tre. Int�ressante � plus d'un points pour ses ressources
min�rales.
	-Theseus, plan�te moyenne, � anneaux elliptiques, � la surface aride et quasi d�sertique. C'est un endroit
id�al pour y dissimuler des activit�s dissidentes.
	-Erebus, petite plan�te verte, � l'atmosph�re vici�e, a priori rendant toute vie organique impossible. Des
sondes ayant cependant enregistr� des signaux sonores �tranges � sa proximit� font suspecter qu'une civilisation extraterrestre intelligente s'y est probablement d�velopp�e (serait-ils responsables du plan de r�volution
inhabituel et non naturel observ� pour cette plan�te ?). 
	-Antaeus, petite plan�te � la surface bleut� par les oc�ans qui la recouvrent totalement. Int�r�t mineur.

Chaque plan�te poss�de sa propre atmosph�re.

Exodus baigne tout le syst�me d'un bruit continu et � tr�s basses fr�quences, si propre � ce type d'astre 
rayonnant et en pleine activit� nucl�aire.

		b) Vaisseaux

On y trouve deux types de vaisseaux :
-les flottes imp�riales et rebelles qui semblent se chasser ind�finiment. 
-un vaisseau extraterrestre (OVNI) circulaire � l'origine encore inconnue, mais suspect� provenir d'Erebus. 
Une entit� sup�rieure ind�termin�e semble provoquer des d�placements sans le moindre sch�ma logique.

Curieusement, malgr� le vide constat� de l'espace, les habitu�s aux voyages interplan�taires t�moignent du bruit
que peuvent faire certains de ces vaisseaux lorsque l'on se trouve � proximit� de ces derniers. Les rebelles semblent �tre parvenus toutefois � trouver un mode de d�placement furtif et non sonoris�, mais � l'origine d'une
�trange projection de lumi�re.

	_________________
	II-2) Interaction

		a) D�placements

Au vu de l'�chelle, il est pr�f�rable d'utiliser les points de vue (clic droit, "Viewpoints") pour se d�placer
d'un objet � l'autre dans la sc�ne. Chaque objet a � cet effet au moins un point de vue qui lui est propre, et 
choisi de telle sorte que l'on ait par la m�me occasion un aper�u du reste du syst�me.
Sinon, le mode de d�placement "Examine" (ic�ne en forme d'oeil en bas � gauche) est appropri�, ainsi que le mode
"Fly" (ic�ne papillon) dans une moindre mesure.

		b) Interaction avec le vaisseau (OVNI)

D'abord, pour appr�cier au mieux cette fonctionnalit�, il est recommand� de choisir le point de vue "Exodus
 Cluster" ou bien "God's eye view" pour avoir une vue d'ensemble et profiter de d�placements facilit�s.

Sur le syst�me se remarque un plan circulaire transparent (si ce n'est pas le cas, modifier le champ de 
transparence, autour de la ligne 650 du fichier "system.wrl") cliquable. En maintenant dessus un clic gauche, il
est possible de faire se d�placer une cible carr�e verte, vers laquelle se dirigera syst�matiquement et
automatiquement le vaisseau-OVNI circulaire gris.

Sa particularit� est qu'il �vitera toutes les plan�tes en d�placement et l'astre central (Exodus) sur son passage :
aucun de ces corps c�lestes n'est traversable par cet objet.

		c) Animations

Les animations automatiques sont de trois sortes :

-chaque plan�te tourne sur elle-m�me et autour de l'�toile Exodus, avec une p�riode de r�volution fonction de sa
distance � cet astre. La lune tourne autour de la Terre.

-l'astre central Exodus simule un rayonnement et une coloration dynamique.

-Des flottes de trois vaisseaux de d�placent p�riodiquement de la plan�te Acheron � la plan�te Theseus (plan�te �
anneaux), pour y att�rir et y d�coller (cela se manifeste visuellement par leur arr�t au-dessus de ces plan�tes
suivi de leur disparition momentan�e). 
Ces vaisseaux se meuvent en gravitant en "spirale" autour d'Exodus pour rejoindre sans encombre leur destination.
Ils y parviendront quelle que soit la position et l'orientation de la plan�te � atteindre � tout moment
(animations non totalement pr�calcul�s, mais adapt�es au contexte), et se d�placent aussi verticalement afin de
 s'adapter au rayon de la plan�te en question (pour se rapprocher de la surface). 


#=================================================================================================================#
#=================================================== Cr�dits =====================================================#

Projet r�alis� par Yohann Rubinsztejn et Micha�l Ludmann dans le cadre de l'option robotique et r�alit� virtuelle 
de 2�me ann�e suivie � l'ENSIIE en 2010.

Enseignement encadr� par M. Guillaume Bouyer.

Note : les fichiers "destroyer.wrl" et "wing.wrl" ne sont pas de notre fait. Pour retrouver leurs sources, se
r�ferer aux en-t�tes de ces fichiers.