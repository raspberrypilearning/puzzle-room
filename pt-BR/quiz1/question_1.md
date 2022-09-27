## Quick quiz

Answer the three questions. There are hints to guide you to the correct answer.

When you have answered each question, click on **Check my answer**.

Have fun!

--- question ---

---
legenda: Pergunta 1 de 3
---

Here is the Monet character next to a big button:

![monet character standing beside a large red button](images/monet-by-button.png)

Which blocks would you use, so that the number of button presses is continually displayed, until the button has been pushed a total of 7 times?


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

Your script says the number of button presses, however it stops after only 5 button presses.

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

These blocks would only run once at the start of the game, as there is no loop being used.

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

Yes! This script says how many times the button has been pressed each time and says the task is complete after 7 button presses.

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

These blocks would say the number `0` seven times really quickly at the start of the game, as there is no condition checking the value of the variable.

  --- /feedback ---

--- /choices ---

--- /question ---
