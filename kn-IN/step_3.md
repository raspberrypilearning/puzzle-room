## ಬಟನ್‌ ಪಝಲ್

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ಈ ಹಂತದಲ್ಲಿ, ನೀವು ನಿಮ್ಮ ಮೊದಲನೆಯ ಪಝಲ್‌ ಸೇರಿಸುತ್ತೀರಿ, ಅದು ಬಟನ್‌ನ್ನು ನಿರ್ದಿಷ್ಟ ಸಂಖ್ಯೆಗಳ ಬಾರಿ ಒತ್ತುವುದಾಗಿರುತ್ತದೆ.
</div>
<div>
![](images/step_3.gif){:width="300px"}
</div>
</div>

ಆಟವು ಶುರುವಾದಾಗ, ಅದು ಒಂದೇ ಸ್ಥಾನದಲ್ಲಿ ಇರಬೇಕು ಮತ್ತು ಆಟಗಾರನಿಗೆ ಯಾವಾಗಲೂ ಕಾಣಿಸುವಂತೆ ಮುಂದಿನ ಪದರದಲ್ಲಿ ಇರಬೇಕು.

--- task ---

**button** ಸ್ಪ್ರೈಟ್‌ಗೆ ಈ ಕೆಳಗಿನ ಬ್ಲಾಕ್‌ಗಳನ್ನು ಸೇರಿಸಿ.

```blocks3
when flag clicked
forever
go to x: (-225) y (27)
go to [front v] layer //The button is visible
```

--- /task ---

ಪಝಲ್‌ ಪೂರ್ಣಗೊಳ್ಳಲು ಬಟನ್‌ನ್ನು ಹಲವಾರು ಬಾರಿ ಒತ್ತಬೇಕಾಗುತ್ತದೆ. ಇದಕ್ಕೆ, ನಿಮಗೆ ಒತ್ತುವ ಸಂಖ್ಯೆಗಳನ್ನು ಸಂಗ್ರಹಿಸಲು `variable`{:class="block3variables"} ಬೇಕಾಗುತ್ತದೆ.

--- task ---

ಹೊಸ `variable`{:class="block3variables"} ರಚಿಸಿ ಮತ್ತು ಅದನ್ನು `button pressed`{:class="block3variables"} ಎಂದು ಕರೆಯಿರಿ.

--- /task ---

ಆಟದ ಪ್ರಾರಂಭದಲ್ಲಿ, `button pressed`{:class="block3variables"} `0` ಆಗಿರಬೇಕು.

--- task ---

**button** ಸ್ಪ್ರೈಟ್‌ಗೆ ಈ ಕೆಳಗಿನ ಬ್ಲಾಕ್‌ಗಳನ್ನು ಸೇರಿಸಿ.

![ಬಟನ್‌ ಸ್ಪ್ರೈಟ್.](images/button-sprite.png)

```blocks3
when flag clicked
set [button pressed v] to (0) //Button presses set to 0 at start
```

--- /task ---

`repeat until`{:class="block3control"} ಬ್ಲಾಕ್‌ ಒಂದು ಲೂಪ್‌ ಆಗಿದ್ದು ಅದು ನಿರ್ದಿಷ್ಟ ಷರತ್ತು ಪೂರೈಸುವವರೆಗೂ ಪುನರಾವರ್ತನೆಯಾಗುತ್ತದೆ.

**ಆಯ್ಕೆ ಮಾಡಿಕೊಳ್ಳಿ:** ಪಝಲ್‌ನ್ನು ಪರಿಹರಿಸಲು ಬಟನ್‌ನ್ನು ಎಷ್ಟು ಬಾರಿ ಒತ್ತಬೇಕು? ಈ ಉದಾಹರಣೆಯಲ್ಲಿ, ಅದನ್ನು `5` ಬಾರಿ ಒತ್ತಬೇಕು, ಆದರೆ ನೀವು ಬೇರೆ ಸಂಖ್ಯೆಯನ್ನು ಆಯ್ದುಕೊಳ್ಳಬಹುದು.

--- task ---

`repeat until`{:class="block3control"} ಲೂಪ್‌ ಸೇರಿಸಿ, ಮತ್ತು ಅದರ ಷರತ್ತನ್ನು `button pressed`{:class="block3variables"} `equal`{:class="block3operators"} ನ್ನು `5` ಆದಾಗ ಎಂದು ಹೊಂದಿಸಿ.

![ಬಟನ್‌ ಸ್ಪ್ರೈಟ್.](images/button-sprite.png)

```blocks3
when flag clicked
set [button pressed v] to (0)
+ repeat until <(button pressed) = (5)> //Keep repeating until button is pressed 5 times
```

--- /task ---

ಈಗ, ಆಟಗಾರ ಬಟನ್‌ ಒತ್ತಲು ಸಾಧ್ಯವಾಗುತ್ತದೆ. ಆದರೂ ಪಾತ್ರವು ಬಟನ್‌ಗೆ ಹತ್ತಿರವಿದ್ದಾಗ ಮಾತ್ರ ಅವರು ಅದನ್ನು ಒತ್ತಲು ಸಾಧ್ಯವಾಗಬೇಕು!

--- task ---

**button** ಸ್ಪ್ರೈಟ್‌ನ್ನು ಕ್ಲಿಕ್‌ ಮಾಡಿದಾಗ ಪಾತ್ರವು ಬಟನ್‌ಗೆ ಹತ್ತಿರವಿದೆಯೇ ಎಂದು ಪತ್ತೆ ಮಾಡಲು ಬ್ಲಾಕ್‌ಗಳನ್ನು ಸೇರಿಸಿ.

![ಬಟನ್‌ ಸ್ಪ್ರೈಟ್.](images/button-sprite.png)

```blocks3
when this sprite clicked
if <(distance to (Monet v)) < (50)> then
else
```

--- /task ---

ಪಾತ್ರವು ಹತ್ತಿರವಿದ್ದರೆ, ಮತ್ತು ಬಟನ್‌ನ್ನು ಒತ್ತಿದರೆ, ಆಗ `button pressed`{:class="block3variables"} ವೇರಿಯೇಬಲ್‌ನ್ನು ಹೆಚ್ಚಿಸಬಹುದು. ಪಾತ್ರವು ಹತ್ತಿರವಿಲ್ಲದಿದ್ದರೆ, ಪಝಲ್‌ ಮರುಹೊಂದಿಕೆಯಾಗಬೇಕು; ಆಟಗಾರ ಇನ್ನಾವುದಾದರೂ ಪಝಲ್‌ ಪ್ರಯತ್ನಿಸುವ ಮೊದಲು, ಐದು ಬಾರಿ ಸತತವಾಗಿ ಬಟನ್‌ ಒತ್ತಬೇಕು.

**ಸಲಹೆ:** Scratch ನಲ್ಲಿ, ಯಾವುದೇ ಎರಡು ಸ್ಪ್ರೈಟ್‌ಗಳ ನಡುವಿನ ದೂರವನ್ನು ಸ್ಪ್ರೈಟ್‌ಗಳ ಕೇಂದ್ರಗಳಿಂದ ಲೆಕ್ಕಹಾಕಲಾಗುತ್ತದೆ. ಇದರ ಅರ್ಥ ದೊಡ್ಡ ಸ್ಪ್ರೈಟ್‌ಗಳು ಸ್ಪರ್ಶಿಸುತ್ತಿರುವಂತೆ ಕಾಣಬಹುದು, ಆದರೆ ಅವುಗಳ ಕೇಂದ್ರಗಳು ದೂರದಲ್ಲಿಯೇ ಇರಬಹುದು.

--- task ---

`button pressed`{:class="block3variables"} ವೇರಿಯೇಬಲ್‌ನ ಮೌಲ್ಯವನ್ನು ಬದಲಾಯಿಸಲು ಕೋಡ್‌ ಸೇರಿಸಿ.

![ಬಟನ್‌ ಸ್ಪ್ರೈಟ್.](images/button-sprite.png)

```blocks3
when this sprite clicked
if <(distance to (Monet v)) < (50)> then
+ change [button pressed v] by (1) //If close to Monet, then increase button press count
else
+ set [button press v] to (0) //If far from Monet, then reset button press count
```

--- /task ---

--- task ---

**ಪರೀಕ್ಷೆ:** ನಿಮ್ಮ ಪ್ರಾಜೆಕ್ಟ್‌ನ್ನು ರನ್‌ ಮಾಡಿ ಮತ್ತು ಪಾತ್ರವನ್ನು ಬಟನ್‌ಗೆ ಹತ್ತಿರ ಚಲಿಸಿ. ನೀವು ಬಟನ್‌ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿದ ತಕ್ಷಣ, `button pressed`{:class='block3variables'} ವೇರಿಯೇಬಲ್‌ ಹೆಚ್ಚಾಗಬೇಕು. ನೀವು `distance to Monet`{:class='block3sensing'} ನ ಮೌಲ್ಯವನ್ನು ಮೇಲೆ ಅಥವಾ ಕೆಳಗೆ ನಿಮಗೆ ಆ ಸಂಖ್ಯೆ ಅರ್ಥಪೂರ್ಣವಾಗಿದೆ ಎನಿಸುವವರೆಗೂ ಹೊಂದಿಸಬಹುದು.

--- /task ---

ನೀವು ಆಟಗಾರನಿಗೆ ಎಷ್ಟು ಬಾರಿ ಬಟನ್‌ ಒತ್ತಲಾಗಿದೆ ಎಂದು `say`{:class="block3looks"} ತಿಳಿಸಲು `join`{:class="block3operators"}ಬ್ಲಾಕ್‌ನ್ನು ಉಪಯೋಗಿಸಬಹುದು.

--- task ---

`join`{:class="block3operators"} ಬ್ಲಾಕ್‌ನ್ನು ಇನ್ನೊಂದರ ಒಳಗೆ ಇಡಿ. ನಂತರ ನಿಮಗೆ ಬೇಕಾದ ಪಠ್ಯವನ್ನು ಮತ್ತು, `button pressed`{:class="block3variables"} ವೇರಿಯೇಬಲ್‌ನ್ನು ಸೇರಿಸಿ, ಎಲ್ಲವೂ `say`{:class="block3looks"} ಬ್ಲಾಕ್‌ ಒಳಗೆ.

ಉದಾಹರಣೆಗೆ:

![ಬಟನ್‌ ಸ್ಪ್ರೈಟ್.](images/button-sprite.png)

```blocks3
when flag clicked
set [button pressed v] to (0)
repeat until <(button pressed) = (5)> 
+ say (join [button pressed] (join (button pressed) [times])
```

**ಸಲಹೆ:** ನಿಮ್ಮ `join`{:class="block3operators"} ಬ್ಲಾಕ್‌ ಒಳಗೆ ಪಠ್ಯಗಳ ನಡುವೆ ಖಾಲಿ ಜಾಗಗಳನ್ನು ಸೇರಿಸಲು ಮರೆಯಬೇಡಿ.

--- /task ---

ಬಟನ್‌ನ್ನು `5` ಬಾರಿ ಒತ್ತಿದಾಗ ಲೂಪ್‌ ಕೊನೆಯಾಗುತ್ತದೆ, ನಂತರ ಬರಹದಲ್ಲಿನ ಕೊನೆಯ ಬ್ಲಾಕ್‌ ರನ್‌ ಆಗುತ್ತದೆ. ಇದು ಆಟಗಾರನಿಗೆ ಕಾರ್ಯವು ಪೂರ್ಣಗೊಂಡಿದೆ ಎಂದು ಹೇಳಬಹುದು.

--- task ---

ಆಟಗಾರನಿಗೆ ಕಾರ್ಯವು ಪೂರ್ಣಗೊಂಡಿದೆ ಎಂದು ಹೇಳಲು `say`{:class="block3looks"} ಬ್ಲಾಕ್‌ ಉಪಯೋಗಿಸಿ.

![ಬಟನ್‌ ಸ್ಪ್ರೈಟ್.](images/button-sprite.png)

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

**ಪರೀಕ್ಷೆ:** ನಿಮ್ಮ ಪ್ರಾಜೆಕ್ಟ್‌ನ್ನು ರನ್‌ ಮಾಡಿ ಮತ್ತು ಪಾತ್ರವನ್ನು ಬಟನ್‌ಗೆ ಹತ್ತಿರ ಚಲಿಸಿ. ನೀವು ಬಟನ್‌ನ್ನು ಐದು ಬಾರಿ ಒತ್ತಿದಾಗ, ಕಾರ್ಯವು ಪೂರ್ಣಗೊಳ್ಳಬೇಕು.

--- /task ---

--- save ---

