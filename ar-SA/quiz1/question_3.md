
--- question ---

---
legend: السؤال 3 من 3
---

انظر إلى المقاطع البرمجي. ما هو أفضل وصف يصف سلوك الكائن الصخري عند النقر على العلم؟


![كائن الصخرة](images/rocks-sprite.png)

```blocks3
when flag clicked
go to (random position v)
repeat until <<touching (sprite 1 v) ?> and <not<touching color (#000000) ?>>
go to (random position v)
```

--- choices ---

- ( )

سيتحرك كائن الصخور إلى موضع عشوائي حتى يلمس **sprite 1** ويلامس اللون الأسود.

  --- feedback ---

ومن شأن هذه الكتل أن تناسب ذلك الوصف. 
<touching (sprite 1 v) ?> و <touching color (#000000) ?>

  --- /feedback ---

- ( )

سيتحرك كائن الصخور إلى موضع عشوائي حتى يلمس **sprite 1** أو لا يلمس اللون الأسود.

  --- feedback ---

<touching (sprite 1 v) ?> أو <not<touching color (#FFFFFF) ?>

  --- /feedback ---

- (x)

سيتحرك الكائن الصخري إلى موضع عشوائي حتى يلمس **sprite 1** ويلامس أي لون آخر غير الأسود.

  --- feedback ---

هذا صحيح. تتحقق الكتلة `وليس`{:class='block3operators'} من أنها لا تلمس اللون الأسود.

  --- /feedback ---

- ( )

سيتحرك كائن الصخور إلى موضع عشوائي حتى لا يلمس **sprite 1** أو اللون الأسود.

  --- feedback ---

<not<touching (sprite 1 v) ?>> أو <touching color (#000000) ?>

  --- /feedback ---

--- /choices ---

--- /question ---
