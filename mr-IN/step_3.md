## बटन पझल

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
या टप्प्यात, तुम्ही तुमचे पहिले कोडे जोडा, ज्यात बटन काही वेळा ढकलायचे असेल.
</div>
<div>
![](images/step_3.gif){:width="300px"}
</div>
</div>

गेम चालू झाल्यावर, बटन त्याच जागी ठेवण्याची आवश्यकता असेल, आणि नेहमी समोरील स्तरावर दिसणे आवश्यक असेल.

--- task ---

**button** स्प्राईटला खालील ब्लॉक्स जोडा.

```blocks3
when flag clicked
forever
go to x: (-225) y (27)
go to [front v] layer //The button is visible
```

--- /task ---

कोडे पूर्ण करण्यासाठी अनेक वेळा बटन ढकलणे आवश्यक असेल. यासाठी, तुम्हाला ढकलण्याची संख्या स्टोअर करण्यासाठी `variable`{:class="block3variables"} ची आवश्यकता असेल.

--- task ---

नवीन `variable`{:class="block3variables"} तयार करा आणि त्याला `button pressed`{:class="block3variables"} म्हणा.

--- /task ---

गेमच्या सुरूवातीला, `button pressed`{:class="block3variables"} हे `0` असायला हवे.

--- task ---

खालील ब्लॉक्स **button** स्प्राईटला जोडा.

![button स्प्राईट.](images/button-sprite.png)

```blocks3
when flag clicked
set [button pressed v] to (0) //Button presses set to 0 at start
```

--- /task ---

`repeat until`{:class="block3control"} ब्लॉक लूप आहे जो विशीष्ट स्थिती जुळेपर्यंत पुनरावृत्ती करतो.

**निवडा:** कोडे सोडविण्यासाठी बटन किती वेळा दाबायचे? या उदाहरणात, तुम्हा ते `5` वेळा दाबावे लागेल, परंतु तुम्ही वेगवेगळी संख्या निवडू शकता.

--- task ---

`repeat until`{:class="block3control"} लूप जोडा, आणि स्थिती`button pressed`{:class="block3variables"} केल्यावर `equal`{:class="block3operators"} `5` अशी सेट करा.

![button स्प्राईट.](images/button-sprite.png)

```blocks3
when flag clicked
set [button pressed v] to (0)
+ repeat until <(button pressed) = (5)> //Keep repeating until button is pressed 5 times
```

--- /task ---

आता, प्लेयर बटन ढकलू शकणे आवश्यक आहे. कॅरेक्टर बटनाच्या जवळ असतांना ते तसे करू शकायला हवे!

--- task ---

**button** स्प्राईटवर क्लिक केल्यावर कॅरेक्टर बटनाच्या जवळ आहे का हे ओळखण्यासाठी ब्लॉक्स जोडा.

![button स्प्राईट.](images/button-sprite.png)

```blocks3
when this sprite clicked
if <(distance to (Monet v)) < (50)> then
else
```

--- /task ---

कॅरेक्टर जवळ असल्यास, आणि बटन दाबल्यास, `button pressed`{:class="block3variables"} व्हेरिएबल वाढवला जाऊ शकतो. कॅरेक्टर जवळ नसल्यास, कोडे रीसेट करायला हवे, प्लेयरने इतर कोणत्याही कोड्याचा प्रयत्न करण्याआधी बटन ओळीत पाच वेळा दाबायला हवे.

**टीप:** Scratch मध्ये, कोणत्याही दोन स्प्राईट्स मधील अंतर स्प्राईटच्या मध्यभागातून काढले जाते. याचा अर्थ, मोठे स्प्राईट्स स्पर्श करत असल्याचे दिसू शकतात, परंतु त्यांचा मध्यभाग दूर असू शकतो.

--- task ---

व्हेरिएबल `button pressed`{:class="block3variables"} ची व्हॅल्यू बदलण्यासाठी कोड जोडा.

![button स्प्राईट.](images/button-sprite.png)

```blocks3
when this sprite clicked
if <(distance to (Monet v)) < (50)> then
+ change [button pressed v] by (1) //Monet जवळ असल्यास, बटन दाबण्याची संख्या वाढवा
else
+ set [button press v] to (0) //Monet पासून लांब असल्यास, बटन दाबण्याची संख्या रीसेट करा
```

--- /task ---

--- task ---

**चाचणी:** तुमचा प्रोजेक्ट रन करा आणि बटनाच्या जवळ कॅरेक्टर हलवा. तुम्ही बटनवर क्लिक केल्यावर, `button pressed`{:class='block3variables'} व्हेरिएबल वाढायला हवा. तुम्ही `distance to Monet`{:class='block3sensing'} ची व्हॅल्यू वर आणि खाली ऍडजस्ट करू शकता, जोपर्यंत तुम्हाला अर्थपूर्ण संख्या सापडत नाही तोपर्यंत.

--- /task ---

तुम्ही `join`{:class="block3operators"} ब्लॉकचा वापर करू शकता प्लेयरला किती वेळा बटन दाबले ते `say`{:class="block3looks"} साठी.

--- task ---

`join`{:class="block3operators"} ब्लॉक दुसऱ्याच्या आत ठेवा. त्यानंतर तुम्हाला हव्या त्या टेक्स्टमध्ये, आणि `button pressed`{:class="block3variables"} व्हेरिएबमध्ये जोडा, सर्व `say`{:class="block3looks"} ब्लॉकच्या आत.

उदाहरणार्थ:

![button स्प्राईट.](images/button-sprite.png)

```blocks3
when flag clicked
set [button pressed v] to (0)
repeat until <(button pressed) = (5)> 
+ say (join [button pressed] (join (button pressed) [times])
```

**टीप:** तुम्ही तुमच्या `join`{:class="block3operators"} ब्लॉकमधील टेक्स्ट मध्ये स्पेस जोडण्याची खात्री करा.

--- /task ---

बटन `5` वेळा दाबल्यावर लूप समाप्त होईल, त्यानंतर स्क्रिप्ट मधील शेवटचा ब्लॉक रन होईल. यामुळे प्लेयरला कार्य पूर्ण झाल्याचे सांगितले जाऊ शकते.

--- task ---

`say`{:class="block3looks"} ब्लॉक प्लेयरला कार्य पूर्ण झाल्याचे सांगण्यासाठी वापरला जातो.

![button स्प्राईट.](images/button-sprite.png)

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

**चाचणी:** तुमचा प्रोजेक्ट रन करा आणि बटनच्या जवळ कॅरेक्टर रन करा. तुम्ही बटनवर पाच वेळा क्लिक केल्यावर, कार्य पूर्ण व्हायला हवे.

--- /task ---

--- save ---

