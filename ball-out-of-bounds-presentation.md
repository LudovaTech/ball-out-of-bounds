# Ball out of bounds
<sup>*memory access out of bounds*</sup>  
*Une mission vous a été confiée, à vous et à votre équipe, par les organisateurs de la Robocup. Cette célèbre compétition, fenêtre sur une robotique de pointe, doit démarrer dans trois semaines. Pourtant, un rôle clé n'a pas pu être pourvu : lors de la compétition, les équipes soccer sont rassemblées dans une zone proche des terrains où elles peuvent travailler, et de nombreuses balles sont laissées entre chaque match sur les terrains.*  
**Vous devez concevoir un robot franchissant la zone de travail grâce à un chemin balisé au préalable, puis, une fois arrivé au terrain, poussant toutes les balles qui s'y trouvent en dehors.**  
*Cependant, pour assurer un maximum de garantie dans cette mission essentielle, une autre équipe a également été désignée pour réaliser la même tâche. Vous devez donc mettre en avant votre talent en robotique en concevant un robot plus performant, capable d'accomplir cette tâche en un temps réduit par rapport à l'autre équipe.*

## Informations techniques

Le parcours est constitué de deux zones mesurant approximativement 1x1 m chacune et accolées.  
La première est un chemin constitué d'une bande noire de 2 cm d'épaisseur formant des tours et des boucles. Votre robot doit suivre ce chemin. Le sol est de couleur blanche.  
Ce chemin mène à la deuxième zone, un sol de couleur verte sur lequel sont placées des balles de golf orange. Toutes les balles orange doivent être poussées en dehors du sol vert. Le carré de sol vert (1x1 m) est entouré d'une bordure de 10 cm de couleur blanche.

## Points

Les scores sont constitués du temps en secondes mis par le robot pour compléter le parcours. Il est possible d'avoir un score négatif ; le but est d'avoir le plus **petit** score possible. Il y a différents malus et bonus :

Sur la zone du chemin noir :
- L'équipe peut décider à n'importe quel moment de replacer son robot sur la dernière ligne noire qu'il a parcourue. Cela rajoute *+10 s*.
- Si le robot sort de la zone, l'équipe est obligée de remettre le robot sur la dernière ligne noire qu'il a parcourue, et cela rajoute *+10 s*.
- Certains passages du parcours peuvent être sautés à la décision de l'équipe. Cela rajoute *+Xs* selon la valeur indiquée sur l'élèment sauté du parcours.

Sur la zone du terrain avec les balles :
- L'équipe peut décider à n'importe quel moment de replacer son robot à l'entrée du terrain. Cela rajoute *+10 s*.
- Si le robot sort de la zone blanche entourant le terrain vert, l'équipe est obligée de remettre le robot à l'entrée du terrain, et cela rajoute *+10 s*.
- Pousser une balle en dehors du terrain enlève *20 s*.
- Le challenge se termine au bout de 10min, chaque balle non ramassée rajoute *+15s*.

## Divers

Pour vous inciter à explorer ce repo GitHub de fond en comble, nous avons caché 4 indices pouvant vous aider dans la conception du robot.
Par exemple, nous annoncer que vous devez rester pour une pièce de théâtre juste avant la compétition vous enlèvera *35s*.
