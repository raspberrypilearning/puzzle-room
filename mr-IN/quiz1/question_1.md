## परावर्तन

छान, तुम्ही खूप काही शिकलात! आता, चिंतन करण्याची वेळ आहे - चिंतन हा अभ्यासाचा महत्वाचा भाग आहे, कारण त्यामुळे तुमच्या मेंदूला नवीन माहिती मिळण्यास मदत होते.

तुम्ही काय शिकलात याचे चिंतन करण्यासाठी खालील तीन प्रश्नांची उत्तरे द्या.

प्रत्येक प्रश्नानंतर submit दाबा. तुम्हाला योग्य उत्तराचे मार्गदर्शन केले जाईल. तुम्हाला हवे तेवढ्या वेळा तुम्ही ही कृती करू शकता.

मजा करा!

--- question ---

---
legend: प्रश्न 3 पैकी 1
---

येथे एका मोठ्या बटणाच्या पुढे Monet कॅरेक्टर आहे:

![मोठ्या लाल बटनच्या बाजूा उभे monet कॅरेक्टर](images/monet-by-button.png)

तुम्ही कोणते ब्लॉक्स वापराल, जेणेकरून बटन एकूण 7 वेळा दाबेपर्यंत किती वेा बटन दाबले हे सतत दिसेल?


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

तुमची स्क्रिप्ट बटन दाब्याची संख्या सांगते, तरीसुद्धा ती केव 5 बटन दाब्यानंतरच थांबते.

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

हे ब्लॉक्स गेमच्या सुरुवातीला फक्त एकदाच चालतील, कारण कोणताही लूप वापरला जात नाही.

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

हो! ही स्क्रिप्ट प्रत्येक वेळी किती वेळा बटण दाबले आहे ते सांगते आणि 7 बटण दाबल्यानंतर कार्य पूर्ण झाल्याचे सांगते.

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

हे ब्लॉक्स गेमच्या अगदी सुरूवातीला तात्काळ `0` संख्या सात वेळा म्हणेल, कारण त्यात व्हेरिएबची व्हॅल्यू तपासण्यासाठी कोणतीही स्थिती नाही.

  --- /feedback ---

--- /choices ---

--- /question ---
