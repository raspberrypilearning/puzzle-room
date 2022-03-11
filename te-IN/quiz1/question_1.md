## పునశ్చరణ

బాగా చేసారు, మీరు చాలా నేర్చుకున్నారు! ఇప్పుడు, విశ్లేషించే సమయం వచ్చింది — విశ్లేషించడం అనేది నేర్చుకోవడంలో ముఖ్యమైన భాగం, ఎందుకంటే ఇది మీ మెదడులో కొత్త కనెక్షన్‌లను ఏర్పరచడంలో సహాయపడుతుంది.

మీరు నేర్చుకున్న వాటిని పరిశీలించడానికి దిగువ మూడు ప్రశ్నలకు సమాధానం ఇవ్వండి.

ప్రతి ప్రశ్న తర్వాత, సబ్మిట్ నొక్కండి. మీరు సరైన సమాధానం వైపు మార్గనిర్దేశం చేయబడతారు. మీరు ఈ చర్యను మీకు కావలసినన్ని సార్లు చేయవచ్చు.

ఆస్వాదించండి!

--- question ---

---
legend: 3లో 1వ ప్రశ్న
---

ఇక్కడ పెద్ద బటన్ పక్కన Monet కారెక్టర్ ఉంది:

![పెద్ద ఎరుపు బటన్ పక్కన నిలబడి ఉన్న monet కారెక్టర్](images/monet-by-button.png)

బటన్ మొత్తం 7 సార్లు పుష్ చేయబడే వరకు బటన్ ప్రెస్‌ల సంఖ్య నిరంతరం ప్రదర్శించబడేలా మీరు ఏ బ్లాక్‌లను ఉపయోగిస్తారు?


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

మీ స్క్రిప్ట్ బటన్ ప్రెస్‌ల సంఖ్యను చెబుతుంది, అయితే ఇది కేవలం 5 బటన్ ప్రెస్‌ల తర్వాత ఆగిపోతుంది.

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

లూప్ ఉపయోగించబడనందున ఈ బ్లాక్‌లు ఆట ప్రారంభంలో ఒకసారి మాత్రమే అమలు చేయబడతాయి.

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

అవును! ఈ స్క్రిప్ట్ ప్రతిసారీ బటన్‌ను ఎన్నిసార్లు నొక్కబడినదో చెబుతుంది మరియు 7 బటన్ ప్రెస్‌ల తర్వాత పని పూర్తయిందని చెబుతుంది.

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

వేరియబుల్ విలువను తనిఖీ చేసే కండిషన్ లేనందున ఈ బ్లాక్‌లు ఆట ప్రారంభంలో `0` సంఖ్యను ఏడుసార్లు త్వరగా చెబుతాయి.

  --- /feedback ---

--- /choices ---

--- /question ---
