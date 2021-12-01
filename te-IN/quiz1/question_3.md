
--- question ---

---
legend: Question 3 of 3
---

Look at the blocks below. Which description best describes the behaviour of the rocks sprite, when the flag is clicked?


![rock sprite](images/rocks-sprite.png)
```blocks3
when flag clicked
go to (random position v)
repeat until <<touching (sprite 1 v) ?> and <not<touching color (#000000) ?>>
go to (random position v)
```

--- choices ---

- ( )

The rocks sprite will move to a random position until it is touching **sprite 1** and touching the colour black.

  --- feedback ---

These blocks would fit that description. <touching (sprite 1 v) ?> and <touching color (#000000) ?>

  --- /feedback ---

- ( )

The rocks sprite will move to a random position until it is touching **sprite 1** or not touching the colour black.

  --- feedback ---

<touching (sprite 1 v) ?> or <not<touching color (#FFFFFF) ?>

  --- /feedback ---

- (x)

The rocks sprite will move to a random position until it is touching **sprite 1** and touching any colour other than black.

  --- feedback ---

Yes, that's correct. The `not`{:class='block3operators'} block checks that it is not touching black.

  --- /feedback ---

- ( )

The rocks sprite will move to a random position until it is not touching **sprite 1** or the colour black.

  --- feedback ---

<not<touching (sprite 1 v) ?>> or <touching color (#000000) ?>

  --- /feedback ---

--- /choices ---

--- /question ---
