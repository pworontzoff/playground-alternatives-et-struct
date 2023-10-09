# Exercice 8

Ecrire un programme qui demande à l’utilisateur d’entrer les 3 côtés a, b, c d’un triangle et qui, si c’est bien un triangle, affiche si ce triangle est isocèle et/ou rectangle et/ou équilatéral.

**Attention : un triangle n'est possible que si l'inégalité triangulaire est respectée. Ce qui veut dire que la somme des longueurs de deux côtés est toujours plus grande que la longueur du troisième côté**

Petite aide :
 - Pour vérifier qu'un triangle est rectangle, on doit s'assurer que la propriété a² = b² + c² est vérifiée pour un des 3 cas possibles (a² = b² + c² ou b² = a² + c² ou c² = a² + b²).
 - Attention, car des erreurs d'arrondis vont très souvent conduire à conclure que x² n'est pas = à y² + z², simplement parce que les calculs faits par le processeurs ne sont pas exacts (ils ne sauraient jamais l'être pour tous les nombres).
 - Pour solutionner le point précédent, il faut :
    1) avoir le plus possible de précision (de décimales correctes) en entrée pour a, b et c et donc ces variables doivent être de type double (avec code de format %lf pour les scanf)
    1) avant de comparer les valeurs données par a² d'une part et par (b² + c²) d'autre part (ou les 2 autres versions), il faudra **caster le résultat en float** ce qui permettra de perdre de la précision, et c'est exactement ce qui nous arrange car dans ce cas, en perdant la précision, nous perdons aussi les erreurs d'arrondis !

Exemples / Tests :
- triangle impossible : a=1 b=2 c=4
- triangle isocèle : a=3 b=3 c=2.6
- triangle équilatéral : a=1 b=1 c=1
- triangle rectangle : a=3 b=4 c=5
- triangle rectangle et isocèle: a=1 b=1 c=1.41421356
- triangle quelconque : a=3 b=3.1 c=2.5

NB : pour le test du triangle rectangle et isocèle, c doit être de type double (avec code de format %lf dans le scanf).