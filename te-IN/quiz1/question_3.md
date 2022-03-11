
--- question ---

---
legend: 3లో 3వ ప్రశ్న
---

దిగువ బ్లాక్‌లను చూడండి. జెండాను క్లిక్ చేసినప్పుడు rocks sprite యొక్క ప్రవర్తనను ఏ వివరణ ఉత్తమంగా వివరిస్తుంది?


![rock sprite](images/rocks-sprite.png)
```blocks3
when flag clicked
go to (random position v)
repeat until <<touching (sprite 1 v) ?> and <not<touching color (#000000) ?>>
go to (random position v)
```

--- choices ---

- ( )

Rocks sprite **sprite 1** ని మరియు నలుపు రంగును తాకే వరకు యాదృచ్ఛిక స్థానానికి తరలించబడుతుంది.

  --- feedback ---

ఈ బ్లాక్‌లు ఆ వివరణకు సరిపోతాయి. <touching (sprite 1 v) ?> మరియు <touching color (#000000) ?>

  --- /feedback ---

- ( )

Rocks sprite **sprite 1** ని లేదా నలుపు రంగును తాకని వరకు యాదృచ్ఛిక స్థానానికి తరలించబడుతుంది.

  --- feedback ---

<touching (sprite 1 v) ?> లేదా <not<touching color (#FFFFFF) ?>

  --- /feedback ---

- (x)

Rocks sprite **sprite 1** ని మరియు నలుపు రంగు కాక ఏదైనా రంగును తాకే వరకు యాదృచ్ఛిక స్థానానికి తరలించబడుతుంది.

  --- feedback ---

అవును, అది సరైనది. `not`{:class='block3operators'} బ్లాక్ అది నలుపును తాకలేదని తనిఖీ చేస్తుంది.

  --- /feedback ---

- ( )

Rocks sprite **sprite 1** ని లేదా నలుపు రంగును తాకని వరకు యాదృచ్ఛిక స్థానానికి తరలించబడుతుంది.

  --- feedback ---

<not<touching (sprite 1 v) ?>> or <touching color (#000000) ?>

  --- /feedback ---

--- /choices ---

--- /question ---
