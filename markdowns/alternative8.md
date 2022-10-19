# Exercice 8

Ecrire un programme qui demande à l’utilisateur d’entrer les 3 côtés a, b, c d’un triangle et qui, si c’est bien un triangle, affiche si ce triangle est isocèle et/ou rectangle et/ou équilatéral.

Exemples / Tests :
- triangle impossible : a=1 b=2 c=4
- triangle isocèle : a=3 b=3 c=2.6
- triangle équilatéral : a=1 b=1 c=1
- triangle rectangle : a=3 b=4 c=5
- triangle rectangle et isocèle: a=1 b=1 c=1.41421356237309504
- triangle quelconque : a=3 b=3.1 c=2.5

NB : pour le test du triangle rectangle et isocèle, c doit être de type double (avec code de format %lf dans le scanf).