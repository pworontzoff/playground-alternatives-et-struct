# Exercice 4

Cet exercice est la suite de l’exercice de localisation d’un DEA ([Série 2 (les variables) - Exercice 6](https://tech.io/playgrounds/55269/2---les-variables/exercice-6)). Modifiez votre programme afin de permettre à l’utilisateur du programme d’encoder les informations degrés, minutes, secondes dans une structure.

Il faut écrire 2 fonctions permettant de faciliter la vie de l’utilisateur :

<ol>
<li> 
Une fonction convertissant des coordonnées géographiques de degrés décimaux en radians.

```math
radian = dd \times \left( \frac{\pi}{180} \right)
```

</li>
<li>
Une fonction convertissant des degrés, minutes, secondes en degrés décimaux.
<ul>
<li>
Si les coordonnées sont positives :

```math
dd = Degrees + \left( \frac{Minutes}{60} \right) + \left( \frac{Secondes}{3600} \right)
```

</li>
<li>
Si les coordonnées sont négatives :

```math
dd = Degrees - \left( \frac{Minutes}{60} \right) - \left( \frac{Secondes}{3600} \right)
```

</li>
</li>
</ol>

NB : 
- Les latitudes Nord et longitudes Est ont des degrés positifs. Les latitudes Sud et longitudes Ouest ont des degrés négatifs.
- L'utilisateur pourrait notamment encoder un angle négatif sous la forme 0° -39' 42" ou 0° 0' -42" 
- Les degrés et les minutes sont des nombres entiers et les secondes peuvent être des réels.

Voici des valeurs de tests pour vérifier que ça fonctionne :

- Latitude de A : 50° 39' 42"
- Longitude de A : 5° 31' 23"
- Latitude de B : 49° 0' 3"
- Longitude de B : 3° 24' 48"
- -> distance entre A et B : 238.753402 (km);