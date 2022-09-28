## Questionnaire rapide

Réponds aux trois questions. Il y a des indices pour te guider vers la bonne réponse.

Lorsque tu as répondu à chaque question, clique sur **Vérifier ma réponse**.

Amuse-toi bien !

--- question ---

---
legend : Question 1 sur 3
---

Voici le personnage Monet à côté d'un gros bouton :

![personnage Monet debout à côté d'un gros bouton rouge](images/monet-by-button.png)

Quels blocs utiliserais-tu pour que le nombre de pressions sur le bouton soit affiché en permanence, jusqu'à ce que le bouton ait été enfoncé 7 fois au total ?


--- choices ---

- ( )

```blocks3
when flag clicked
set [button pressed v] to (0)
repeat until <(button pressed) = (5)>
say (button pressed)
end
say [task complete] for (2) seconds
```

  --- feedback ---

Ton script indique le nombre de pressions sur le bouton, mais il s'arrête après seulement 5 pressions sur le bouton.

  --- /feedback ---

- ( )

```blocks3
when flag clicked
set [button pressed v] to (0)
if <(button pressed) > (6)> then
say (button pressed)
end
say [task complete] for (2) seconds
```

  --- feedback ---

Ces blocs ne fonctionneraient qu'une seule fois au début du jeu, car aucune boucle n'est utilisée.

  --- /feedback ---

- (x)

```blocks3
when flag clicked
set [button pressed v] to (0)
repeat until <(button pressed) > (6)>
say (button pressed)
end
say [task complete] for (2) seconds
```

  --- feedback ---

Oui ! Ce script indique combien de fois le bouton a été enfoncé à chaque fois et indique que la tâche est terminée après 7 pressions sur le bouton.

  --- /feedback ---

- ( )

```blocks3
when flag clicked
set [button pressed v] to (0)
repeat (7)
say (button pressed)
end
say [task complete)] for (2) seconds
```
  --- feedback ---

Ces blocs diraient le nombre `0` sept fois très rapidement au début du jeu, car il n'y a pas de condition vérifiant la valeur de la variable.

  --- /feedback ---

--- /choices ---

--- /question ---
