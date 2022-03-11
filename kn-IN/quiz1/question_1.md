## ಪುನರ್ಮನನ

ಭೇಷ್, ನೀವು ಬಹಳಷ್ಟು ಕಲಿತಿದ್ದೀರಿ! ಈಗ ಪುನರ್ಮನನ ಮಾಡುವ ಸಮಯ — ಪುನರ್ಮನನ ಕಲಿಕೆಯ ಒಂದು ಮಹತ್ವದ ಭಾಗ, ಏಕೆಂದರೆ ಅದು ನಿಮ್ಮ ಮೆದುಳಿನಲ್ಲಿ ಹೊಸ ಸಂಪರ್ಕಗಳನ್ನು ಮಾಡಲು ಸಹಾಯ ಮಾಡುತ್ತದೆ.

ನೀವು ಕಲಿತಿದ್ದನ್ನು ಪುನರ್ಮನನ ಮಾಡಲು ಈ ಕೆಳಗಿನ ಮೂರು ಪ್ರಶ್ನೆಗಳಿಗೆ ಉತ್ತರಿಸಿ.

ಪ್ರತಿಯೊಂದು ಪ್ರಶ್ನೆಯ ನಂತರ, ಸಬ್ಮಿಟ್‌ ಒತ್ತಿ. ಸರಿಯಾದ ಉತ್ತರದ ಕಡೆಗೆ ನಿಮಗೆ ಮಾರ್ಗದರ್ಶನ ನೀಡಲಾಗುತ್ತದೆ. ಈ ಚಟುವಟಿಕೆಯನ್ನು ನೀವು ಎಷ್ಟು ಸಲ ಬೇಕಾದರೂ ಮಾಡಬಹುದು.

ಆನಂದಿಸಿ!

--- question ---

---
legend: ಪ್ರಶ್ನೆ 3 ರಲ್ಲಿ 1
---

ದೊಡ್ಡ ಬಟನ್‌ ಪಕ್ಕ ಇಲ್ಲಿ Monet ಪಾತ್ರ ಇದೆ:

![ದೊಡ್ಡ ಕೆಂಪು ಬಟನ್‌ ಪಕ್ಕ ನಿಂತಿರುವ monet ಪಾತ್ರ](images/monet-by-button.png)

ಬಟನ್‌ನ್ನು ಒಟ್ಟು 7 ಬಾರಿ ಒತ್ತಲಾಗುವವರೆಗೆ, ಒತ್ತಲಾದ ಬಟನ್‌ಗಳ ಸಂಖ್ಯೆಯನ್ನು ನಿರಂತರವಾಗಿ ಪ್ರದರ್ಶಿಸುವಂತೆ ಮಾಡಲು ನೀವು ಯಾವ ಬ್ಲಾಕ್‌ಗಳನ್ನು ಉಪಯೋಗಿಸುತ್ತೀರಿ?


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

ನಿಮ್ಮ ಬರಹ ಒತ್ತಲಾದ ಬಟನ್‌ಗಳ ಸಂಖ್ಯೆಯನ್ನು ಹೇಳುತ್ತದೆ, ಅದರೆ ಅದು 5 ಬಟನ್‌ಗಳು ಒತ್ತಲ್ಪಟ್ಟಾಗ ನಿಲ್ಲುತ್ತದೆ.

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

ಈ ಬ್ಲಾಕ್‌ಗಳು ಆಟದ ಪ್ರಾರಂಭದಲ್ಲಿ ಒಮ್ಮೆ ಮಾತ್ರ ರನ್‌ ಆಗುತ್ತವೆ ಏಕೆಂದರೆ ಇಲ್ಲಿ ಯಾವುದೇ ಲೂಪ್‌ ಬಳಸಿಲ್ಲ.

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

ಹೌದು! ಈ ಬರಹ ಪ್ರತಿಬಾರಿ ಬಟನ್‌ನ್ನು ಎಷ್ಟು ಸಲ ಒತ್ತಲಾಗಿದೆ ಎಂದು ಹೇಳುತ್ತದೆ ಮತ್ತು 7 ಬಟನ್‌ ಒತ್ತಲಾದ ನಂತರ ಕಾರ್ಯ ಪೂರ್ಣಗೊಂಡಿದೆ ಎಂದು ಹೇಳುತ್ತದೆ.

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

ವೇರಿಯೇಬಲ್‌ನ ಮೌಲ್ಯವನ್ನು ಪರಿಶೀಲಿಸುವ ಯಾವುದೇ ಷರತ್ತು ಇಲ್ಲವಾದುದರಿಂದ ಈ ಬ್ಲಾಕ್‌ಗಳು ಆಟದ ಪ್ರಾರಂಭದಲ್ಲಿ ಸಂಖ್ಯೆಯನ್ನು `0` ಏಳು ಬಾರಿ ಬಹಳ ಬೇಗ ಹೇಳುತ್ತವೆ.

  --- /feedback ---

--- /choices ---

--- /question ---
