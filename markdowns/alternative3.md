# Exercice 3

La structure suivante est définie :

```c 
struct date {
	int jour;
	int mois;
	int annee;
};
```

Il faut écrire un programme qui permet d'encoder une date (saisie du jour, puis du mois, puis de l'année) et qui affiche la date entrée sous la forme JJ/MM/AAAA. Par exemple :

```html
Encodage d'une date
jour : 6
mois : 12
annee : 1945

Date encodee : 06/12/1945
```
**Remarque:** Pour affichage de la date les zéros initiaux pour les jours et mois doivent apparaître. La syntaxe suivant peut être utilisée dans le `printf` : `%02d`. Cela signifie qu'on affiche au moins 2 caractères en remplissant avec des 0 si nécéssaire.

```C runnable
#include <stdlib.h>
#include <stdio.h>

int main() {
	
	printf("%05d\n",123);
	printf("%02d\n",5);
	printf("%02d\n",12);

	return 0;
}
```