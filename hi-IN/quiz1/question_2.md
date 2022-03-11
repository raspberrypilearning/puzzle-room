
--- question ---

---
legend: 3 में से दूसरा प्रश्न
---

हैंडव्हील पहेली के लिए यहां एक स्क्रिप्ट दी गई है:

```blocks3
when flag clicked
set [turned v] to (0)
set [handwheel turned v] to (0)
repeat until <(handwheel turned) > (2)>
end
say [task complete] for (2) seconds
```

एक पूर्ण वाक्य का उपयोग करते हुए, चरित्र को यह बताने के लिए कि उन्होंने कितनी बार पहिया घुमाया है, आप स्क्रिप्ट में कोड की कौन सी पंक्ति जोड़ेंगे?

--- choices ---

- (x)

```blocks3
say (join [handwheel turned ] (join (handwheel turned) [ times])
```

  --- feedback ---

हाँ, अगर हैंडव्हील तीन बार घुमाया गया है तो यह कहेगा `handwheel turned 3 times`{:class='block3looks'}।

  --- /feedback ---

- ( )

```blocks3
say (join [handwheel turned ]  [ times])
```

  --- feedback ---

इस स्क्रिप्ट के साथ अगर हैंडव्हील को 3 बार माया गया है तो यह कहेगा `handwheel turned times`{:class='block3looks'}

  --- /feedback ---

- ( )

```blocks3
say (join (handwheel turned)(join [handwheel turned ] [times])
```

  --- feedback ---

इस स्क्रिप्ट के साथ अगर हैंडव्हील को 3 बार घुमाया गया है तो यह कहेगा `3 handwheel turned times`{:class='block3looks'}

  --- /feedback ---

- ( )

```blocks3
say (handwheel turned)
```
  --- feedback ---

इस स्क्रिप्ट के साथ अगर हैंडव्हील को 3 बार घुमाया गया है तो यह कहेगा `3`{:class='block3looks'}

  --- /feedback ---

--- /choices ---

--- /question ---
