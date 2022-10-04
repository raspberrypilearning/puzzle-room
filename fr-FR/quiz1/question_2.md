
--- question ---

---
legend: Question 2 sur 3
---

Voici un script pour un puzzle de gouvernail :

```blocks3
when flag clicked
set [a tourné v] to (0)
set [gouvernail a tourné v] to (0)
repeat until <(gouvernail a tourné) > (2)>
end
say [tâche terminée] for (2) seconds
```

Quelle ligne de code ajouterais-tu au script pour dire au personnage combien de fois il a tourné la roue, en utilisant une phrase complète ?

--- choices ---

- (x)

```blocks3
say (join [gouvernail a tourné ] (join (gouvernail a tourné) [ fois])
```

  --- feedback ---

Oui, si le gouvernail avait été tourné 3 fois, il aurait dit `gouvernail a tourné 3 fois`{:class='block3looks'}

  --- /feedback ---

- ( )

```blocks3
say (join [gouvernail a tourné ]  [ fois])
```

  --- feedback ---

Avec ce script, si le gouvernail avait été tourné 3 fois, il aurait dit `gouvernail a tourné fois`{:class='block3looks'}

  --- /feedback ---

- ( )

```blocks3
say (join (gouvernail a tourné)(join [gouvernail a tourné ] [fois])
```

  --- feedback ---

Avec ce script, si le gouvernail avait été tourné 3 fois, il aurait dit `3 fois gouvernail a tourné`{:class='block3looks'}

  --- /feedback ---

- ( )

```blocks3
say (gouvernail a tourné)
```
  --- feedback ---

Avec ce script, si le gouvernail avait été tourné 3 fois, il aurait dit `3`{:class='block3looks'}

  --- /feedback ---

--- /choices ---

--- /question ---
