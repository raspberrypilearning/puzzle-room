## सोचिए

बहुत बढ़िया, आपने बहुत कुछ सीखा! अब, अब उस पर विचार करने का समय है - विचार करना सीखने का एक महत्वपूर्ण हिस्सा है, क्योंकि यह आपके दिमाग को तेज़ करता है।

आपने जो सीखा है उस पर चिंतन करने के लिए नीचे दिए गए तीन प्रश्नों के उत्तर दें।

प्रत्येक प्रश्न के बाद, सबमिट करें दबाएं। यह आपको सही उत्तर की तरफ लेकर जाएगा। आप इस गतिविधि को जितनी बार चाहें उतनी बार कर सकते हैं।

मजे करें!

--- question ---

---
legend: 3 में से पहला प्रश्न
---

यहाँ एक बड़े बटन के बगल में Monet चरित्र है:

![monet चरित्र एक बड़े लाल बटन के पास खड़ा है](images/monet-by-button.png)

आप किन ब्लॉकों का उपयोग करेंगे, ताकि बटन दबाने की संख्या लगातार प्रदर्शित हो, जब तक कि बटन को कुल 7 बार दबाया न जाए?


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

आपकी स्क्रिप्ट बटन दबाने की संख्या कहती है, हालांकि यह केवल 5 बार बटन दबाने के बाद बंद हो जाती है।

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

ये ब्लॉक खेल की शुरुआत में केवल एक बार चलेंगे, क्योंकि इसमें लूप का उपयोग नहीं किया जा रहा है।

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

हाँ! यह स्क्रिप्ट कहती है कि हर बार कितनी बार बटन दबाया गया है और कि 7 बार बटन दबाने के बाद कहती है कार्य पूरा हो गया है।

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

खेल के शुरू में ये ब्लॉक गिनती `0` सात बार वास्तव में तेजी से कहेंगे, क्योंकि वेरिएबल के मान की जाँच करने की कोई शर्त नहीं है।

  --- /feedback ---

--- /choices ---

--- /question ---
