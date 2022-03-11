
--- question ---

---
legend: 3 में से तीसरा प्रश्न
---

नीचे दिए गए ब्लॉकों को देखें। जब झंडे को क्लिक किया जाता है, तो कौन सा विवरण रॉक्स स्प्राइट के व्यवहार का सबसे अच्छा वर्णन करता है?


![rock स्प्राइट](images/rocks-sprite.png)
```blocks3
when flag clicked
go to (random position v)
repeat until <<touching (sprite 1 v) ?> and <not<touching color (#000000) ?>>
go to (random position v)
```

--- choices ---

- ( )

रॉक्स स्प्राइट एक यादृच्छिक स्थिति में तब तक चला जाएगा जब तक कि यह < **sprite 1** को स्पर्श न कर रहा हो और काले रंग को छू रहा हो।

  --- feedback ---

ये ब्लॉक उस विवरण में फिट होंगे। 
<touching (sprite 1 v) ?> और <touching color (#000000) ?>

  --- /feedback ---

- ( )

रॉक स्प्राइट एक यादृच्छिक स्थिति में तब तक चला जाएगा जब तक कि यह **sprite 1** को स्पर्श न कर रहा हो या काले रंग को नहीं छू रहा हो।

  --- feedback ---

<touching (sprite 1 v) ?> or <not<touching color (#FFFFFF) ?>

  --- /feedback ---

- (x)

रॉक्स स्प्राइट एक यादृच्छिक स्थिति में तब तक चला जाएगा जब तक कि वह **sprite 1** को स्पर्श न कर ले और काले रंग के अलावा किसी अन्य रंग को न छू ले।

  --- feedback ---

हाँ, यह सही है। `not`{:class='block3operators'} ब्लॉक जांचता है कि यह काला तो नहीं छू रहा है।

  --- /feedback ---

- ( )

रॉक स्प्राइट एक यादृच्छिक स्थिति में चला जाएगा जब तक कि यह **sprite 1** या काले रंग को नहीं छू रहा हो।

  --- feedback ---

<not<touching (sprite 1 v) ?>> or <touching color (#000000) ?>

  --- /feedback ---

--- /choices ---

--- /question ---
