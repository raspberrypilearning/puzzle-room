
--- question ---

---
legend: Cwestiwn 3 o 3
---

Cymer olwg ar y blociau isod. Pa ddisgrifiad sy'n disgrifio ymddygiad corlun Rocks orau, pan gaiff y faner ei chlicio?


![corlun craig](images/rocks-sprite.png)
```blocks3
when flag clicked
go to (random position v)
repeat until <<touching (sprite 1 v) ?> and <not<touching color (#000000) ?>>
go to (random position v)
```

--- choices ---

- ( )

Bydd corlun Rocks yn symud i safle ar hap nes ei fod yn cyffwrdd â **sprite 1** ac yn cyffwrdd â'r lliw du.

  --- feedback ---

Byddai'r blociau hyn yn cyd-fynd â'r disgrifiad hwnnw. <touching (sprite 1 v) ?> a <touching color (#000000) ?>

  --- /feedback ---

- ( )

Bydd corlun Rocks yn symud i safle ar hap nes ei fod yn cyffwrdd â **sprite 1** neu heb gyffwrdd â'r lliw du.

  --- feedback ---

<touching (sprite 1 v) ?> neu <ddim<touching color (#FFFFFF) ?>

  --- /feedback ---

- (x)

Bydd corlun Rocks yn symud i safle ar hap nes ei fod yn cyffwrdd â **sprite 1** ac yn cyffwrdd ag unrhyw liw heblaw du.

  --- feedback ---

Cywir. Mae'r bloc `ddim`{:class='block3operators'} yn gwirio nad yw'n cyffwrdd â du.

  --- /feedback ---

- ( )

Bydd corlun Rocks yn symud i safle ar hap nes ei fod ddim yn cyffwrdd â **sprite 1** neu'r lliw du.

  --- feedback ---

<not<touching (sprite 1 v) ?>> or <touching color (#000000) ?>

  --- /feedback ---

--- /choices ---

--- /question ---
