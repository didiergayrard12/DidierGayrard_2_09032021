# DidierGayrard_2_09032021
Repo for OC PR2

Quelques commentaires sur le design:
Vous trouverez en ligne le folder "design" ou j'ai fait mes relevés de dimensions et de layout en mode "grille"
J'ai ajouté aussi le schéma block de décaupage de la maquette en balise sémantiques HTML.
Une des différences de l'implemantation par rapport a ce schéma block c'est ue j'ai découpé la section  des activités en deux sous section pour faire une pagination plus fine pour les tablettes

Mes breapoints sont :
1370 pixels, qui correspondent ala zone ou on vient "écraser" la section des activites

1024 pixels qui est le breakpoint courant pour les tablettes

700 pixels pour les formats smartphones, qui correspond aussi a la zone ou le div "actblock" n'a plus de place 
on en profite donc pour tout mettre en mode colonne

Les points notables du design:
1) la section activités est découpée en div qui permettent de faire une mise en colonne a deux niveaux , un pour un element "actblock" au nombre de deux dans le layout qui vienent se mettre en coolonne au breakpoint 1370 , pendant que le reste est inchangé.


2) a 1024 pixels, c'est la liste des poulaires qui passe devant en colonne avec la liste des hébergements

3) a 700 pixels tout se retrouve en colonne

4) j'ai choisi de ne pas faire de thumbnails pour ce layout
J'utilise un concept de "viewport" entre la zone ou afficher la photo et la photo elle même
la photo "img" est positionnée en absolute sur le viewport "aphoto" ou "hphoto" ou "hpphoto" ou "lpphoto" et ces dernieres "class" recoivent un param position:relative
J'ai utilisé pour toutes les photos le folder 4_small


NOTE: j'ai stocké dans des folders "*_thumb_*" des images adaptéees aux differents formats du layout mais je ne les ai pas encore utilisées

Je prévois de faire une branche pour exploiter ces images.

TESTS éffectués sur cette version:

Firefox: parcours 
https://didiergayrard12.github.io/DidierGayrard_2_09032021/index.html
avec toutes largeurs et largeur maximum plus appui bouton fentre entiere et reduction

Chrome:
idem plus essai de diverses format de tablettes

BUGS a FIXER et LIMITATIONS:
1) probleme vu sur les deux : décalage a droite de la section Activités : FIXED
2) pas de marges sur header avec logo et boutton s'inscrire : FIXED
3) tablettes et smartphones: scroll possible de droite a gauche: A comprendre si c'est une limitation

LIMITATION 3 FIXED: missing position:absolute on an hidden object was causing overflow






