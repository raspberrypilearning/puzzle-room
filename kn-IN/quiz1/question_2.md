
--- question ---

---
legend: ಪ್ರಶ್ನೆ 2 ರಲ್ಲಿ 3
---

ಕೈಚಕ್ರ ಪಜಲ್‌ಗೆ ಇಲ್ಲಿ ಒಂದು ಬರಹವಿದೆ:

```blocks3
when flag clicked
set [turned v] to (0)
set [handwheel turned v] to (0)
repeat until <(handwheel turned) > (2)>
end
say [task complete] for (2) seconds
```

ಸಂಪೂರ್ಣ ವಾಕ್ಯವನ್ನು ಉಪಯೋಗಿಸಿ, ಪಾತ್ರಕ್ಕೆ ಅವುಗಳು ಎಷ್ಟು ಬಾರಿ ಚಕ್ರವನ್ನು ತಿರುಗಿಸಿದವು ಎಂದು ಹೇಳಲು, ಬರಹಕ್ಕೆ ಯಾವ ಕೋಡ್‌ ಲೈನ್‌ ಸೇರಿಸುತ್ತೀರಿ?

--- choices ---

- (x)

```blocks3
say (join [handwheel turned ] (join (handwheel turned) [ times])
```

  --- feedback ---

ಹೌದು, ಕೈಚಕ್ರವನ್ನು 3 ಬಾರಿ ತಿರುಗಿಸಿದ್ದರೆ ಅದು `handwheel turned 3 times`{:class='block3looks'} ಎಂದು ಹೇಳುತ್ತದೆ

  --- /feedback ---

- ( )

```blocks3
say (join [handwheel turned ]  [ times])
```

  --- feedback ---

ಈ ಬರಹದಿಂದ, ಕೈಚಕ್ರವನ್ನು 3 ಬಾರಿ ತಿರುಗಿಸಿದ್ದರೆ ಅದು `handwheel turned times`{:class='block3looks'} ಎಂದು ಹೇಳುತ್ತದೆ,

  --- /feedback ---

- ( )

```blocks3
say (join (handwheel turned)(join [handwheel turned ] [times])
```

  --- feedback ---

ಈ ಬರಹದಿಂದ, ಕೈಚಕ್ರವನ್ನು 3 ಬಾರಿ ತಿರುಗಿಸಿದ್ದರೆ ಅದು `3 handwheel turned times`{:class='block3looks'} ಎಂದು ಹೇಳುತ್ತದೆ

  --- /feedback ---

- ( )

```blocks3
say (handwheel turned)
```
  --- feedback ---

ಈ ಬರಹದಿಂದ, ಕೈಚಕ್ರವನ್ನು 3 ಬಾರಿ ತಿರುಗಿಸಿದ್ದರೆ ಅದು <0>3</0> {:class='block3looks'} ಎಂದು ಹೇಳುತ್ತದೆ

  --- /feedback ---

--- /choices ---

--- /question ---
