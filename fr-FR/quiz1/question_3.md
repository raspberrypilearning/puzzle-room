
--- question ---

---
legend : Question 3 sur 3
---

Regarde les blocs ci-dessous. Quelle description décrit le mieux le comportement du sprite des rochers, lorsque le drapeau est cliqué ?


![sprite Météore](images/rocks-sprite.png)
```blocks3
when flag clicked
go to (random position v)
repeat until <<touching (sprite 1 v) ?> and <not<touching color (#000000) ?>>
go to (random position v)
```

--- choices ---

- ( )

Le sprite des rochers se déplacera vers une position aléatoire jusqu'à ce qu'il touche **sprite 1** et touche la couleur noire.

  --- feedback ---

Ces blocs correspondraient à cette description. <touching (sprite 1 v) ?> et <touching color (#000000) ?>

  --- /feedback ---

- ( )

Le sprite des rochers se déplacera vers une position aléatoire jusqu'à ce qu'il touche **sprite 1** ou ne touche pas la couleur noire.

  --- feedback ---

<touching (sprite 1 v) ?> ou "&#060" ; non<touching color (#FFFFFF) ?>

  --- /feedback ---

- (x)

Le sprite des rochers se déplacera vers une position aléatoire jusqu'à ce qu'il touche **sprite 1** et touche une couleur autre que la couleur noire.

  --- feedback ---

Oui c'est correct. Le bloc `pas`{:class='block3operators'} vérifie qu'il ne touche pas le noir.

  --- /feedback ---

- ( )

Le sprite des rochers se déplacera vers une position aléatoire tant qu'il ne touche pas **sprite 1** ou la couleur noire.

  --- feedback ---

<not<touching (sprite 1 v) ?>> or <touching color (#000000) ?>

  --- /feedback ---

--- /choices ---

--- /question ---
