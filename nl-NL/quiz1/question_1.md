## Snelle quiz

Beantwoord de drie vragen. Er zijn tips om je naar het juiste antwoord te leiden.

Wanneer je elke vraag hebt beantwoord, klik je op **Verzenden**.

Veel plezier!

--- question ---

---
legend: Vraag 1 van 3
---

Hier is het Monet-personage naast een grote knop:

![het Monet-personage dat naast een grote rode knop staat](images/monet-by-button.png)

Welke blokken zou je gebruiken, zodat het aantal keren dat op de knop wordt gedrukt continu wordt weergegeven totdat de knop in totaal 7 keer is ingedrukt?


--- choices ---

- ( )

```blocks3
when flag clicked
set [knop ingedrukt v] to (0)
repeat until <(knop ingedrukt) = (5)>
say (knop ingedrukt)
end
say [opdracht voltooid] for (2) seconds
```

  --- feedback ---

Je script geeft het aantal keer dat op een knop wordt gedrukt weer, maar stopt na slechts 5 keer drukken.

  --- /feedback ---

- ( )

```blocks3
when flag clicked
set [knop ingedrukt v] to (0)
if <(knop ingedrukt) > (6)> then
say (knop ingedrukt)
end
say [opdracht voltooid] for (2) seconds
```

  --- feedback ---

Deze blokken zouden slechts eenmaal aan het begin van het spel lopen, omdat er geen lus wordt gebruikt.

  --- /feedback ---

- (x)

```blocks3
when flag clicked
set [knop ingedrukt v] to (0)
repeat until <(knop ingedrukt) > (6)>
say (knop ingedrukt)
end
say [opdracht voltooid] for (2) seconds
```

  --- feedback ---

Ja! Dit script geeft weer hoe vaak de knop is ingedrukt en zegt dat de opdracht is voltooid nadat de knop 7 keer is ingedrukt.

  --- /feedback ---

- ( )

```blocks3
when flag clicked
set [knop ingedrukt v] to (0)
repeat (7)
say (knop ingedrukt)
end
say [opdracht voltooid)] for (2) seconds
```
  --- feedback ---

Deze blokken zouden het getal `0` zeven keer heel snel aan het begin van het spel laten zien, omdat er geen voorwaarde is om de waarde van de variabele te controleren.

  --- /feedback ---

--- /choices ---

--- /question ---
