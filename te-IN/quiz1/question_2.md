
--- question ---

---
legend: 3లో 2వ ప్రశ్న
---

హ్యాండ్‌వీల్ పజిల్ కోసం స్క్రిప్ట్ ఇక్కడ ఉంది:

```blocks3
when flag clicked
set [turned v] to (0)
set [handwheel turned v] to (0)
repeat until <(handwheel turned) > (2)>
end
say [task complete] for (2) seconds
```

పూర్తి వాక్యాన్ని ఉపయోగించి, కారెక్టర్ ఎన్నిసార్లు చక్రం తిప్పిందో చెప్పడానికి మీరు స్క్రిప్ట్‌కి ఏ లైన్ కోడ్‌ను జోడిస్తారు?

--- choices ---

- (x)

```blocks3
say (join [handwheel turned ] (join (handwheel turned) [ times])
```

  --- feedback ---

అవును, హ్యాండ్‌వీల్‌ను 3 సార్లు తిప్పినట్లయితే అది `handwheel turned 3 times`{:class='block3looks'} అని చెప్తుంది

  --- /feedback ---

- ( )

```blocks3
say (join [handwheel turned ]  [ times])
```

  --- feedback ---

ఈ స్క్రిప్ట్‌తో హ్యాండ్‌వీల్‌ను 3 సార్లు తిప్పినట్లయితే, అది `handwheel turned times`{:class='block3looks'} అని చెప్తుంది

  --- /feedback ---

- ( )

```blocks3
say (join (handwheel turned)(join [handwheel turned ] [times])
```

  --- feedback ---

ఈ స్క్రిప్ట్‌తో హ్యాండ్‌వీల్‌ను 3 సార్లు తిప్పినట్లయితే, అది `3 handwheel turned times`{:class='block3looks'} అని చెప్తుంది

  --- /feedback ---

- ( )

```blocks3
say (handwheel turned)
```
  --- feedback ---

ఈ స్క్రిప్ట్‌తో హ్యాండ్‌వీల్‌ను 3 సార్లు తిప్పినట్లయితే, అది `3`{:class='block3looks'} అని చెప్తుంది

  --- /feedback ---

--- /choices ---

--- /question ---
