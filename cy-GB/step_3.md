## Pos y botwm

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Yn y cam hwn, byddi di'n ychwanegu dy bos cyntaf, sef gwthio'r botwm nifer penodol o weithiau.
</div>
<div>
![](images/step_3.gif){:width="300px"}
</div>
</div>

Pan fydd y gêm yn dechrau, mae angen i'r botwm aros yn yr un lle, a bod yn weladwy bob amser ar yr haen flaen.

--- task ---

Ychwanegu'r blociau canlynol at y corlun **botwm**.

```blocks3
when flag clicked
forever
go to x: (-225) y (27)
go to [front v] layer //The button is visible
```

--- /task ---

Bydd angen gwthio'r botwm nifer o weithiau er mwyn cwblhau'r pos. Ar gyfer hyn, bydd angen `newidyn`{:class="block3variables"} arnat i storio nifer y gwthiadau.

--- task ---

Crea `newidyn`{:class="block3variables"} a'i alw'n `botwm wedi'i wasgu`{:class="block3variables"}.

--- /task ---

Ar ddechrau'r gêm, dylai `botwm wedi'i wasgu`{:class="block3variables"} fod yn `0`.

--- task ---

Ychwanega'r blociau canlynol at y corlun **botwm**.

![Corlun y botwm.](images/button-sprite.png)

```blocks3
when flag clicked
set [button pressed v] to (0) //Button presses set to 0 at start
```

--- /task ---

Mae bloc `ailadrodd tan`{:class="block3control"} yn ddolen sy'n parhau i ailadrodd nes bod amod penodol wedi'i fodloni.

**Dewisa:** Sawl gwaith fydd angen pwyso'r botwm i ddatrys y pos? Yn yr enghraifft hon, bydd angen ei wasgu `5` gwaith, ond gelli ddewis rhif gwahanol.

--- task ---

Ychwanega ddolen `ailadrodd tan`{:class="block3control"}, a gosod ei gyflwr i fod pan fydd `botwm yn cael ei wasgu`{:class="block3variables"} yn `gyfartal`{:class="block3operators"} i `5`.

![Corlun y botwm.](images/button-sprite.png)

```blocks3
when flag clicked
set [button pressed v] to (0)
+ repeat until <(button pressed) = (5)> //Keep repeating until button is pressed 5 times
```

--- /task ---

Nawr, mae angen i'r chwaraewr allu gwthio'r botwm. Ond dim ond pan fydd y cymeriad yn agos at y botwm y dylen nhw allu ei wasgu!

--- task ---

Ychwanega flociau i ganfod a yw'r cymeriad yn agos at y botwm pan fydd **botwm** y corlun yn cael ei glicio.

![Corlun y botwm.](images/button-sprite.png)

```blocks3
when this sprite clicked
if <(distance to (Monet v)) < (50)> then
else
```

--- /task ---

Os yw'r cymeriad yn agos, a'r botwm yn cael ei wasgu, yna gellir cynyddu'r newidyn `botwm wedi'i wasgu`{:class="block3variables"}. Os nad yw'r cymeriad yn agos, dylai'r pos ailosod; mae angen i'r chwaraewr wthio'r botwm bum gwaith yn olynol, cyn rhoi cynnig ar unrhyw bosau eraill.

**Awgrym:** Yn Scratch, mae'r pellter rhwng unrhyw ddau gorlun yn cael ei gyfrifo o ganol y corlun. Mae hyn yn golygu y gall corlun mawr edrych fel pe baent yn cyffwrdd, ond efallai bod eu canol yn dal i fod ymhell oddi wrth ei gilydd.

--- task ---

Ychwanega god i newid gwerth y newidyn `botwm wedi'i wasgu`{:class="block3variables"}.

![Corlun y botwm.](images/button-sprite.png)

```blocks3
when this sprite clicked
if <(distance to (Monet v)) < (50)> then
+ change [button pressed v] by (1) //If close to Monet, then increase button press count
else
+ set [button pressed v] to (0) //If far from Monet, then reset button press count
```

--- /task ---

--- task ---

**Profi:** Rheda dy brosiect a symud y cymeriad yn agos at y botwm. Wrth i ti glicio ar y botwm, dylai'r newidyn `botwm wedi'i wasgu`{:class='block3variables'} gynyddu. Gelli addasu gwerth `pellter i Monet`{:class='block3sensing'} i fyny neu i lawr, nes i ti ddod o hyd i rif sy'n gwneud synnwyr i ti.

--- /task ---

Gelli ddefnyddio'r bloc `ymuno`{:class="block3operators"} i `ddweud`{:class="block3looks"} i'r chwaraewr sawl gwaith mae'r botwm wedi'i wasgu.

--- task ---

Gosoda floc `ymuno`{:class="block3operators"} y tu mewn i un arall. Yna ychwanega'r testun rwyt ti ei eisiau, a'r newidyn `botwm wedi'i wasgu`{:class="block3variables"}, i gyd y tu mewn i floc `dweud`{:class="block3looks"}.

Er enghraifft:

![Corlun y botwm.](images/button-sprite.png)

```blocks3
when flag clicked
set [button pressed v] to (0)
repeat until <(button pressed) = (5)> 
+ say (join [button pressed] (join (button pressed) [times])
```

**Awgrym:** Gwna'n siŵr dy fod yn ychwanegu bylchau yn y testun yn dy floc `ymuno`{:class="block3operators"}.

--- /task ---

Bydd y ddolen yn dod i ben pan fydd y botwm wedi'i wasgu `5` gwaith, yna bydd y bloc olaf yn y sgript yn cael ei redeg. Gall hyn ddweud wrth y chwaraewr bod y dasg wedi'i chwblhau.

--- task ---

Defnyddia floc `dweud`{:class="block3looks"} i ddweud wrth y chwaraewr bod y dasg wedi'i chwblhau.

![Corlun y botwm.](images/button-sprite.png)

```blocks3
when flag clicked
set [button pressed v] to (0)
repeat until <(button pressed) = (5)>
say (join [button pressed] (join (button pressed) [times])
end
+ say [task complete] for (2) seconds
```

--- /task ---



--- task ---

**Profi:** Rheda dy brosiect a symud y cymeriad yn agos at y botwm. Pan fyddi di'n clicio ar y botwm bum gwaith, dylai'r dasg fod yn gyflawn.

--- /task ---

--- save ---

