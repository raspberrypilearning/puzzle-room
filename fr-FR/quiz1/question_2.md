
--- question ---

---
legend : Question 2 sur 3
---

Voici un script pour un puzzle de gouvernail :

```blocks3
when flag clicked
set [turned v] to (0)
set [handwheel turned v] to (0)
repeat until <(handwheel turned) > (2)>
end
say [task complete] for (2) seconds
```

Quelle ligne de code ajouterais-tu au script pour dire au personnage combien de fois il a tourné la roue, en utilisant une phrase complète ?

--- choices ---

- (x)

```blocks3
say (join [handwheel turned ] (join (handwheel turned) [ times])
```

  --- feedback ---

Oui, si le gouvernail avait été tourné 3 fois, il aurait dit `gouvernail tourné 3 fois`{:class='block3looks'}

  --- /feedback ---

- ( )

```blocks3
say (join [handwheel turned ]  [ times])
```

  --- feedback ---

Avec ce script, si le gouvernail avait été tourné 3 fois, il aurait dit ` gouvernail tourné fois`{:class='block3looks'}

  --- /feedback ---

- ( )

```blocks3
say (join (handwheel turned)(join [handwheel turned ] [times])
```

  --- feedback ---

Avec ce script, si le gouvernail avait été tourné 3 fois, il aurait dit `3 fois gouvernail tourné`{:class='block3looks'}

  --- /feedback ---

- ( )

```blocks3
say (handwheel turned)
```
  --- feedback ---

Avec ce script, si le gouvernail avait été tourné 3 fois, il aurait dit `3`{:class='block3looks'}

  --- /feedback ---

--- /choices ---

--- /question ---
