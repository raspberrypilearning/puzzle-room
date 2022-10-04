
--- question ---

---
legend: Vraag 2 van 3
---

Hier is een script voor een wielpuzzel:

```blocks3
when flag clicked
set [gedraaid v] to (0)
set [wiel gedraaid v] to (0)
repeat until <(wiel gedraaid) > (2)>
end
say [opdracht voltooid] for (2) seconds
```

Welke coderegel zou je aan het script toevoegen om het personage, met een volledige zin, te vertellen hoe vaak ze het wiel hebben gedraaid?

--- choices ---

- (x)

```blocks3
say (join [wiel ] (join (wiel gedraaid) [ keer gedraaid])
```

  --- feedback ---

Ja, als het wiel 3 keer was gedraaid zou het `wiel 3 keer gedraaid`{:class='block3looks'} zeggen

  --- /feedback ---

- ( )

```blocks3
say (join [wiel ]  [ keer gedraaid])
```

  --- feedback ---

Als het wiel 3 keer gedraaid was zou dit script `wiel keer gedraaid`{:class='block3looks'} zeggen

  --- /feedback ---

- ( )

```blocks3
say (join (wiel gedraaid)(join [wiel ] [keer gedraaid])
```

  --- feedback ---

Als het wiel 3 keer gedraaid was met dit script zou het `3 keer gedraaid wiel`{:class='block3looks'} zeggen

  --- /feedback ---

- ( )

```blocks3
say (wiel gedraaid)
```
  --- feedback ---

Als het wiel 3 keer gedraaid was zou dit script `3`{:class='block3looks'} zeggen

  --- /feedback ---

--- /choices ---

--- /question ---
