## Handwheel పజిల్

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ఈ దశలో, మీరు హ్యాండ్‌వీల్‌ను తిప్పాల్సిన పజిల్‌ని సృష్టిస్తారు.
</div>
<div>
![](images/step_4.gif){:width="300px"}
</div>
</div>

ఈ పజిల్‌కి సంబంధించిన స్క్రిప్ట్‌లు button పజిల్‌తో సమానంగా ఉంటాయి, కాబట్టి మీరు ఆ స్క్రిప్ట్‌లను కాపీ చేసి, ఆపై వాటిని సవరించవచ్చు.

--- task ---

మీరు **button** sprite కోసం సృష్టించిన రెండు స్క్రిప్ట్‌లను **handwheel** sprite కు డ్రాగ్ చేయండి, వాటిని ఆ sprite కి కాపీ చేయండి.

--- /task ---

`when flag clicked`{:class='block3events'} స్క్రిప్ట్, మార్చవలసిన వాటిలో మొదటిది.

--- task ---

`handwheel turned`{:class="block3variables"} అనబడే కొత్త వేరియబుల్ ని సృష్టించండి, మరియు దానిని `button pressed`{:class="block3variables"} వేరియబుల్ కి బదులుగా ఉపయోగించండి.

**ఎంచుకోండి:** పూర్తి సంఖ్యను మీరు ఎలా ఉండాలనుకుంటున్నారో దానికి మార్చండి. మనము ఉదాహరణలో `3` ని ఎంచుకున్నాము.

![Handwheel sprite.](images/handwheel-sprite.png)

```blocks3
when flag clicked
+ set [handwheel turned v] to (0)
+ repeat until <(handwheel turned) = (3)>
+ say (join [handwheel turned] (join (handwheel turned) [times])
end
+ say [task complete] for (2) seconds
```

--- /task ---

నిజమైన హ్యాండ్‌వీల్ లాగా, **handwheel** sprite ఒక సమయంలో తక్కువ సంఖ్యలో మాత్రమే డిగ్రీలను తిప్పగలదు, కాబట్టి అది తిప్పబడిన కోణాన్ని నిల్వ చేయాలి.

--- task ---

`turned`{:class="block3variables"} అనే కొత్త వేరియబుల్‌ని సృష్టించండి మరియు గేమ్ ప్రారంభమైనప్పుడు దాన్ని `0` కి సెట్ చేయండి.

![Handwheel sprite.](images/handwheel-sprite.png)

```blocks3
when flag clicked
+ set [turned v] to (0)
set [handwheel turned v] to (0)
repeat until <(handwheel turned) = (3)>
say (join [handwheel turned] (join (handwheel turned) [times])
end
say [task complete] for (2) seconds
```

--- /task ---

ఇప్పుడు మీరు ఈ `when this sprite clicked`{:class="block3events"} స్క్రిప్ట్‌ను సవరించవచ్చు, తద్వారా **handwheel** sprite ని పదే పదే క్లిక్ చేసినప్పుడు అది పూర్తి పరిక్రమణం పూర్తి చేసే వరకు ప్రతిసారీ చిన్న మొత్తంలో తిరుగుతుంది. ఇది సరైన సంఖ్యలో పూర్తి పరిక్రమణలను పూర్తి చేసినప్పుడు (ఉదాహరణలో`3` సార్లు), పజిల్ పరిష్కరించబడుతుంది.

--- task ---

**handwheel** sprite క్లిక్ చేయబడిన ప్రతిసారీ, అది `15` డిగ్రీలు తిరుగుతుంది మరియు `turned`{:class="block3variables"} వేరియబుల్ `15` వరకు పెరుగుతుంది.

![Handwheel sprite.](images/handwheel-sprite.png)

```blocks3
when this sprite clicked
if <(distance to (Monet v)) < (50)> then
+ change [turned v] by (15) //Store the turnes of the wheel
+ turn cw (15) degrees
else
+ set [handwheel turned v] to (0)
```

--- /task ---

**పరీక్ష**: **Monet** sprite (లేదా మీ కారెక్టర్ sprite) ని **handwheel** కి దగ్గరగా తరలించి, ఆపై **handwheel** sprite పై క్లిక్ చేయండి. ఇది పూర్తి స్క్రీన్ మోడ్‌లో ఉండటానికి సహాయపడుతుంది, తద్వారా మీరు **handwheel** sprite చుట్టూ డ్రాగ్ చేయండి.

`turned`{:class="block3variables"} వేరియబుల్ `360`కి చేరుకున్నప్పుడు, handwheel ఒకసారి తిప్పబడుతుంది; ఇది ఇప్పుడు `handwheel turned`{:class="block3variables"} వేరియబుల్‌లో నిల్వ చేయబడుతుంది.

--- task ---

`handwheel turned`{:class="block3variables"}ని మార్చడానికి **nested** `<code>if`{:class="block3control"} ని ఉపయోగించండి మరియు <1>turned</code>{:class="block3variables"} వేరియబుల్‌లను రీసెట్ చేయండి. `if`{:class="block3control"} ని మరొక దాని లోపల ఉంచినప్పుడు దానిని A **nested** `if`{:class="block3control"} అంటారు.

![Handwheel sprite.](images/handwheel-sprite.png)

```blocks3
when this sprite clicked
if <(distance to (Monet v)) < (50)> then
change [turned v] by (15)
turn cw (15) degrees
+ if <(turned) = (360)> then //The handwheel has turned a full circle
+ change [handwheel turned v] by (1) //Store the total number of turns
+ set [turned v] to (0) //Reset the angle that it has been turned
end
else
set [handwheel turned v] to (0)
```

--- /task ---

--- task ---

**పరీక్ష:** మీ క్యారెక్టర్ sprite ని హ్యాండ్‌వీల్‌కి దగ్గరగా తరలించి, ఆపై దానిపై క్లిక్ చేయండి. హ్యాండ్‌వీల్ నుండి కారెక్టర్ ఉండాల్సిన దూరాన్ని మీరు సర్దుబాటు చేయాల్సి రావచ్చు.

![Handwheel sprite.](images/handwheel-sprite.png)

```blocks3
<(distance to (Monet v)) < (150)>
```

--- /task ---

**చిట్కా**: మీరు మీ **Monet** (లేదా క్యారెక్టర్) spriteని హ్యాండ్‌వీల్‌కి దగ్గరగా తీసుకురావడానికి దాన్ని క్లిక్ చేసి డ్రాగ్ చేయవచ్చు. ఇది మీ సమయాన్ని ఆదా చేస్తుంది, ఎందుకంటే మీరు కంట్రోల్స్ ను ఉపయోగించాల్సిన అవసరం ఉండదు.

--- save ---
