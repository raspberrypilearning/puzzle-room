## हँडव्हील पझल

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
या टप्प्यात, तुम्ही कोडे तयार कराल ज्यात हँडव्हीलने वळणे आवश्यक आहे.
</div>
<div>
![](images/step_4.gif){:width="300px"}
</div>
</div>

या कोड्याची स्क्रिप्ट थोडी बटन पझल सारखीच आहे, त्यामुळे तुम्ही त्या स्क्रिप्ट्स कॉपी करून त्यानंतर त्या एडिट करू शकता.

--- task ---

तुम्ही **button** स्प्राईट आणि **handwheel** स्प्राईटसाठी तुम्ही तयार केलेल्या दोन स्क्रिप्ट्स त्या स्प्राईटला कॉपी करण्यासाठी ड्रॅग करा.

--- /task ---

`when flag clicked`{:class='block3events'} स्क्रिप्ट ही प्रथम आहे ज्यात बदल करणे आवश्यक आहे.

--- task ---

नवीन व्हेरिएबल तयार करा त्याला `handwheel turned`{:class="block3variables"} म्हणा, आणि व्हेरिएबलचा `button pressed`{:class="block3variables"} व्हेरिएबल ऐवजी वापर करा.

**निवडा:** तुम्हाला जे व्हावेसे वाटेल त्यामध्ये कंप्लीशन संख्या बदला. उदाहरणासाठी आपण `3` निवडली.

![handwheel स्प्राईट.](images/handwheel-sprite.png)

```blocks3
when flag clicked
+ set [handwheel turned v] to (0)
+ repeat until <(handwheel turned) = (3)>
+ say (join [handwheel turned] (join (handwheel turned) [times])
end
+ say [task complete] for (2) seconds
```

--- /task ---

खऱ्या हँडव्हीलप्रमाणे, **handwheel** स्प्राईट केवळ एका वेळी कमी प्रमाणातच वळू शकतो, त्यामुळे तो ज्या कोनात वळला ते स्टोअर करणे आवश्यक असेल.

--- task ---

नवीन व्हेरिएबल तयार करा ज्याला `turned`{:class="block3variables"} म्हणतात आणि तो गेमच्या सुरूवातला `0` सेट करा.

![handwheel स्प्राईट.](images/handwheel-sprite.png)

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

आता तुम्ही `when this sprite clicked`{:class="block3events"} स्क्रिप्ट एडिट करू शकता, जेणेकरून जेव्हा **handwheel** स्प्राईट पुन्हा पुन्हा क्लिक केल्या जाईल तो प्रत्येक वेळी चक्र पूर्ण होईपर्यंत थोड्या प्रमाणात वळेल. त्याने पूर्ण वळणाची योग्य संख्या पूर्ण केल्यावर (`3` वेळा उदाहरणासाठी), कोडे सोडवले जाईल.

--- task ---

ब्लॉक्स जोडा जेणेकरून **handwheel** स्प्राईटवर क्लिक केल्यावर, तो `15` डिग्री वळतो आणि `turned`{:class="block3variables"} व्हेरिएबल `15` ने वाढतो.

![handwheel स्प्राईट.](images/handwheel-sprite.png)

```blocks3
when this sprite clicked
if <(distance to (Monet v)) < (50)> then
+ change [turned v] by (15) //Store the turnes of the wheel
+ turn cw (15) degrees
else
+ set [handwheel turned v] to (0)
```

--- /task ---

**चाचणी**: **Monet** स्प्राईट (किंवा तुमचे कॅरेक्टर स्प्राईट) **handwheel** जवळ हलवा आणि त्यानंतर **handwheel** स्प्राईटवर क्लिक करा. यामुळे फुलस्क्रीन मोड होण्यास मदत होते, जेणेकरून तुम्ही तुम्ही **handwheel** स्प्राईट भोवती ड्रॅग करू शकता.

`turned`{:class="block3variables"} व्हेरिएबल `360` वर पोहोचल्यावर, हँडव्हील एकदा वळला; हे आता व्हेरिएबल `handwheel turned`{:class="block3variables"} मध्ये स्टोअर केले जाऊ शकते.

--- task ---

**नेस्टेड** `if`{:class="block3control"} चा `handwheel turned`{:class="block3variables"} बदलण्यासाठी वापर करा आणि `turned`{:class="block3variables"} व्हेरिएबल रीसेट करा. **नेस्टेड** `if`{:class="block3control"} म्हणजे `if`{:class="block3control"} हा दुसऱ्यात आत ठेवला असणे.

![handwheel स्प्राईट.](images/handwheel-sprite.png)

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

**चाचणी:** तुमचा कॅरेक्टर स्प्राईट हँडव्हीलच्या जवळ हलवा, आणि त्यानंतर त्यावर क्लिक करा. कॅरेक्टरला हँडव्हील कडून आवश्यक असलेले अंतर तुम्हाला कदाचीत ऍडजस्ट करावे लागू शकते.

![handwheel स्प्राईट.](images/handwheel-sprite.png)

```blocks3
<(distance to (Monet v)) < (150)>
```

--- /task ---

**टीप**: तुम्ही तुमच्या **Monet** (किंवा कॅरेक्टर) स्प्राईट वर क्लिक करून भोवती ड्रॅग करू शकता, तो क्षणासाठी हँडव्हीलच्या जवळ आणण्यासाठी. हे तुमचा वेळ वाचवेल, कारण तुम्हाला कंट्रोल्स वापरावी लागणार नाहीत.

--- save ---
