## बटन पहेली

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
इस चरण में, आप अपनी पहली पहेली जोड़ेंगे, जो एक निश्चित संख्या में एक बटन को दबाना होगी।
</div>
<div>
![](images/step_3.gif){:width="300px"}
</div>
</div>

जब खेल शुरू होता है, तो बटन को उसी स्थान पर रहना चाहिए, और हमेशा सामने की परत पर दिखाई देना चाहिए।

--- task ---

निम्नलिखित ब्लॉकों को **button** स्प्राइट में जोड़ें।

```blocks3
when flag clicked
forever
go to x: (-225) y (27)
go to [front v] layer //The button is visible
```

--- /task ---

पहेली को पूरा करने के लिए बटन को कई बार दबाना होगा। इसके लिए, आपको एक`variable`{:class="block3variables"} की आवश्यकता होगी ताकि दबाने की संख्या को स्टोर किया जा सके।

--- task ---

एक नया `variable`{:class="block3variables"} बनाएं, जिसे `button pressed`{:class="block3variables"} कहा जाता है।

--- /task ---

खेल की शुरुआत में, `button pressed`{:class="block3variables"} को `0` होना चाहिए ।

--- task ---

निम्नलिखित ब्लॉकों को **button** स्प्राइट में जोड़ें।

![button स्प्राइट.](images/button-sprite.png)

```blocks3
when flag clicked
set [button pressed v] to (0) //Button presses set to 0 at start
```

--- /task ---

`repeat until`{:class="block3control"} वह लूप है जो एक निश्चित शर्त पूरी होने तक दोहराना जारी रखता है।

**चुनें:** पहेली को हल करने के लिए बटन को कितनी बार दबाने की आवश्यकता होगी? इस उदाहरण में, इसे `5` बार दबाने की आवश्यकता होगी, लेकिन आप कोई भिन्न संख्या चुन सकते हैं।

--- task ---

`repeat until`{:class="block3control"} लूप जोड़ें और उसकी शर्त को ऐसे सेट करें की जब `button pressed`{:class="block3variables"} `equal`{:class="block3operators"} के `5` है

![button स्प्राइट.](images/button-sprite.png)

```blocks3
when flag clicked
set [button pressed v] to (0)
+ repeat until <(button pressed) = (5)> //Keep repeating until button is pressed 5 times
```

--- /task ---

अब, खिलाड़ी को बटन दबाने में सक्षम होना चाहिए। हालाँकि वे इसे केवल तभी दबा सकते हैं जब चरित्र बटन के करीब हो!

--- task ---

यह पता लगाने के लिए ब्लॉक जोड़ें कि **button** स्प्राइट क्लिक करने पर चरित्र बटन के करीब है या नहीं।

![button स्प्राइट.](images/button-sprite.png)

```blocks3
when this sprite clicked
if <(distance to (Monet v)) < (50)> then
else
```

--- /task ---

यदि चरित्र पास है, और बटन को दबाया जाता है, तो `button pressed`{:class="block3variables"} वेरिएबल बढ़ाया जा सकता है। यदि चरित्र करीब नहीं है, तो पहेली को रीसेट करना चाहिए; खिलाड़ी को किसी भी अन्य पहेली को आजमाने से पहले लगातार पांच बार बटन दबाने की जरूरत है।

**सलाह:** Scratch में, किन्हीं दो स्प्राइट्स के बीच की दूरी की गणना स्प्राइट्स के केंद्रों से की जाती है। इसका मतलब है कि बड़े स्प्राइट्स ऐसे लग सकते हैं जैसे वे एक दुसरे को छू रहे हों, लेकिन उनके केंद्र अभी भी दूर हो सकते हैं।

--- task ---

वेरिएबल `button pressed`{:class="block3variables"} का मान बदलने के लिए कोड जोड़ें।

![button स्प्राइट.](images/button-sprite.png)

```blocks3
when this sprite clicked
if <(distance to (Monet v)) < (50)> then
+ change [button pressed v] by (1) //If close to Monet, then increase button press count
else
+ set [button press v] to (0) //If far from Monet, then reset button press count
```

--- /task ---

--- task ---

**परिक्षण:** अपना प्रोजेक्ट चलाएँ और चरित्र को बटन के पास ले जाएँ। जैसे ही आप बटन पर क्लिक करते हैं, `button pressed`{:class='block3variables'} वेरिएबल बढ़ जाना चाहिए। आप `distance to Monet`{:class='block3sensing'} के मान को ऊपर या नीचे तक समायोजित कर सकते हैं, जब तक कि आपको कोई ऐसी संख्या न मिल जाए जो आपको उपयुक्त लगे।

--- /task ---

आप `join`{:class="block3operators"} ब्लॉक का उपयोग खिलाडी को यह `say`{:class="block3looks"} के लिए कर सकते हैं कि बटन कितनी बार दबाया गया है।

--- task ---

एक `join`{:class="block3operators"} ब्लॉक को दूसरे के अंदर रखें। फिर अपने इच्छित टेक्स्ट में जोड़ें, और `button pressed`{:class="block3variables"} वेरिएबल सबको `say`{:class="block3looks"} ब्लॉक में रखें ।

उदाहरण के लिए:

![button स्प्राइट.](images/button-sprite.png)

```blocks3
when flag clicked
set [button pressed v] to (0)
repeat until <(button pressed) = (5)> 
+ say (join [button pressed] (join (button pressed) [times])
```

**सलाह:** सुनिश्चित करें कि आप `join`{:class="block3operators"} ब्लॉक में टेक्स्ट के बीच जगह छोड़ते हैं।

--- /task ---

जब बटन `5` बार दबाया गया है लूप समाप्त हो जाएगा, फिर स्क्रिप्ट में अंतिम ब्लॉक चलाया जाएगा। यह खिलाड़ी को बता सकता है कि कार्य पूरा हो गया है।

--- task ---

खिलाड़ी को यह बताने के लिए कि कार्य पूरा हो गया है, `say`{:class="block3looks"} ब्लॉक का उपयोग करें।

![button स्प्राइट.](images/button-sprite.png)

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

**परिक्षण:** अपना प्रोजेक्ट चलाएँ और चरित्र को बटन के पास ले जाएँ। जब आप पांच बार बटन पर क्लिक करते हैं, तो कार्य पूरा हो जाना चाहिए।

--- /task ---

--- save ---

