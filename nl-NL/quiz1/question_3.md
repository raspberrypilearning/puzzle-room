
--- question ---

---
legend: Vraag 3 van 3
---

Kijk naar de blokken hieronder. Welke beschrijving geeft het beste het gedrag van de rocks sprite aan wanneer op de vlag wordt geklikt?


![rock sprite](images/rocks-sprite.png)
```blocks3
when flag clicked
go to (random position v)
repeat until <<touching (sprite 1 v) ?> and <not<touching color (#000000) ?>>
go to (random position v)
```

--- choices ---

- ( )

De rocks sprite beweegt naar een willekeurige positie totdat hij **sprite 1** raakt en de kleur zwart raakt.

  --- feedback ---

Deze blokken zouden bij die beschrijving passen. <touching (sprite 1 v) ?> en <touching color (#000000) ?>

  --- /feedback ---

- ( )

De rocks sprite beweegt naar een willekeurige positie totdat hij **sprite 1** raakt of de kleur zwart niet raakt.

  --- feedback ---

<touching (sprite 1 v) ?> of <niet<touching color (#FFFFFF) ?>

  --- /feedback ---

- (x)

De rocks sprite beweegt naar een willekeurige positie totdat hij **sprite 1** raakt en iedere andere kleur dan zwart raakt.

  --- feedback ---

Ja dat is goed. Het `niet`{:class='block3operators'} blok controleert of het zwart niet raakt.

  --- /feedback ---

- ( )

De rocks sprite beweegt naar een willekeurige positie totdat hij **sprite 1** of de kleur zwart niet raakt.

  --- feedback ---

<not<touching (sprite 1 v) ?>> or <touching color (#000000) ?>

  --- /feedback ---

--- /choices ---

--- /question ---
