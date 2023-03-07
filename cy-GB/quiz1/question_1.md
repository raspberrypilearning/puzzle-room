## Cwis cyflym

Ateba'r tri chwestiwn. Mae awgrymiadau ar gael i dy arwain at yr ateb cywir.

Ar ôl i ti ateb pob cwestiwn, clicia ar **Gwirio fy ateb**.

Mwynha!

--- question ---

---
legend: Cwestiwn 1 o 3
---

Dyma'r cymeriad Monet wrth ymyl botwm mawr:

![cymeriad monet yn sefyll wrth ymyl botwm mawr coch](images/monet-by-button.png)

Pa flociau fyddet ti'n eu defnyddio, fel bod nifer y gwasgfeydd botwm yn cael eu harddangos yn barhaus, nes bod y botwm wedi'i wthio cyfanswm o 7 gwaith?


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

Mae dy sgript yn dweud y nifer o wasgiau botwm, fodd bynnag mae'n stopio ar ôl dim ond 5 gwasg botwm.

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

Dim ond unwaith y byddai'r blociau hyn yn rhedeg ar ddechrau'r gêm, gan nad oes dolen yn cael ei defnyddio.

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

Iawn! Mae'r sgript hon yn dweud sawl gwaith mae'r botwm wedi'i wasgu bob tro ac yn dweud bod y dasg wedi'i chwblhau ar ôl pwyso botwm 7 gwaith.

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

Byddai'r blociau hyn yn dweud y rhif `0` saith gwaith yn gyflym iawn ar ddechrau'r gêm, gan nad oes unrhyw amod yn gwirio gwerth y newidyn.

  --- /feedback ---

--- /choices ---

--- /question ---
