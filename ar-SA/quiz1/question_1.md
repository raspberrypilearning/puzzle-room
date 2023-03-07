## اختبار سريع

أجب على الاسئلة الثلاثة. هناك تلميحات لإرشادك إلى الإجابة الصحيحة.

عندما تجيب على كل سؤال، انقر فوق **تحقق من إجابتي**.

استمتع!

--- question ---

---
القائمة: السؤال 1 من 3
---

هذه هي شخصية Monet بجانب زر كبير:

![monet شخصية تقف بجانب زر أحمر كبير](images/monet-by-button.png)

ما المقاطع البرمجية التي ستستخدمها ، بحيث يتم عرض عدد مرات الضغط على الزر باستمرار ، حتى يتم الضغط على الزر إجمالي 7 مرات؟


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

يوضح االمقطع البرمجي الخاص بك عدد مرات الضغط على الأزرار ، ولكنه يتوقف بعد ضغطات 5 فقط على الأزرار.

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

سيتم تشغيل هذه المقاطع البرمجية مرة واحدة فقط في بداية اللعبة ، حيث لا توجد حلقة مستخدمة.

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

نعم! يوضح هذا المقطع البرمجي عدد مرات الضغط على الزر في كل مرة ويقول إن المهمة قد اكتملت بعد 7 ضغطات على الزر.

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

ستقول هذه المقاطع البرمجية الرقم `0` سبع مرات بسرعة كبيرة في بداية اللعبة ، حيث لا يوجد شرط للتحقق من قيمة المتغير.

  --- /feedback ---

--- /choices ---

--- /question ---
