
--- question ---

---
legend: प्रश्न 3 पैकी 3
---

खालील कोड पहा. झेंड्यावर क्लिक केल्यावर rocks स्प्राईटच्या वागणूकीचे उत्तम वर्णन कोण करेल?


![rocks स्प्राईट](images/rocks-sprite.png)
```blocks3
when flag clicked
go to (random position v)
repeat until <<touching (sprite 1 v) ?> and <not<touching color (#000000) ?>>
go to (random position v)
```

--- choices ---

- ( )

rocks स्प्राईट **sprite 1** ला स्पर्श करेपर्यंत आणि काळ्या रंगाला स्पर्श करेपर्यंत कोणत्याही पोजिशनमध्ये हलेल.

  --- feedback ---

हे ब्लॉक त्या वर्णनात बसतील. <touching (sprite 1 v) ?> आणि <touching color (#000000) ?>

  --- /feedback ---

- ( )

rocks स्प्राईट **sprite 1** ला स्पर्श करेपर्यंत किंवा काळ्या रंगाला स्पर्श करत नाही तोपर्यंत कोणत्याही पोजिशन मध्ये हलेल.

  --- feedback ---

<touching (sprite 1 v) ?> or <not<touching color (#FFFFFF) ?>

  --- /feedback ---

- (x)

rocks स्प्राईट **sprite 1** ला स्पर्श करेपर्यंत किंवा काळा रंग वगळता इतर कोणत्याही रंगाला स्पर्श करत नाही तोपर्यंत कोणत्याही पोजिशन मध्ये हलेल.

  --- feedback ---

हो, ते बरोबर आहे. `not`{:class='block3operators'} ब्लॉक तो काळ्याला स्पर्श करत नसल्याचे तपासतो.

  --- /feedback ---

- ( )

rocks स्प्राईट **sprite 1** ला स्पर्श करेपर्यंत किंवा काळ्या रंगाला स्पर्श करत नाही तोपर्यंत कोणत्याही पोजिशन मध्ये हलेल.

  --- feedback ---

<not<touching (sprite 1 v) ?>> किंवा <touching color (#000000) ?>

  --- /feedback ---

--- /choices ---

--- /question ---
