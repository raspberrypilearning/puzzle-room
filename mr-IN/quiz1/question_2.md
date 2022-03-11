
--- question ---

---
legend: प्रश्न 3 पैकी 2
---

हँडव्हील पझल साठी येथे स्क्रिप्ट आहे:

```blocks3
when flag clicked
set [turned v] to (0)
set [handwheel turned v] to (0)
repeat until <(handwheel turned) > (2)>
end
say [task complete] for (2) seconds
```

पूर्ण वाक्य वापरून कॅरेक्टरने किती वेळा चाक वळवले हे सांगण्यासाठी तुम्ही स्क्रिप्टला कोडची कोणती लाईन जोडाल?

--- choices ---

- (x)

```blocks3
say (join [handwheel turned ] (join (handwheel turned) [ times])
```

  --- feedback ---

हो, हँडव्हील 3 वेळा वळवले तर ते `handwheel turned 3 times`{:class='block3looks'} म्हणेल

  --- /feedback ---

- ( )

```blocks3
say (join [handwheel turned ]  [ times])
```

  --- feedback ---

या स्क्रिप्टसह, हँडव्हील 3 वेळा वळवले तर ते `handwheel turned times`{:class='block3looks'} म्हणेल

  --- /feedback ---

- ( )

```blocks3
say (join (handwheel turned)(join [handwheel turned ] [times])
```

  --- feedback ---

या स्क्रिप्टसह, हँडव्हील 3 वेळा वळवले तर ते `handwheel turned times`{:class='block3looks'} म्हणेल

  --- /feedback ---

- ( )

```blocks3
say (handwheel turned)
```
  --- feedback ---

या स्क्रिप्टसह, हँडव्हील 3 वेळा वळवले तर ते `3`{:class='block3looks'} म्हणेल

  --- /feedback ---

--- /choices ---

--- /question ---
