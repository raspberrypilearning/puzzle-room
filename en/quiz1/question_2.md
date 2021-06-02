
--- question ---

---
legend: Question 2 of 3
---

Here's a script for a handwheel puzzle:

```blocks3
when flag clicked
set [turned v] to (0)
set [handwheel turned v] to (0)
repeat until <(handwheel turned) = (3)>
end
say (task complete) for (2) seconds
```

Which line of code would you add to the script to tell the character how many times they have turned the wheel, using a complete sentence?

--- choices ---

- (x) 
say (join [handwheel turned ] (join (handwheel turned) [ times])
  --- feedback ---
Yes, if the handwheel had been turned 3 times it would say `handwheel turned 3 times`{:class='block3looks'}
  --- /feedback ---

- ( ) 
say (join [handwheel turned ]  [ times])
  --- feedback ---
With this script if the handwheel had been turned 3 times it would say `handwheel turned times`{:class='block3looks'}
  --- /feedback ---

- ( ) 
say (join (handwheel turned)(join [handwheel turned ] [times])
  --- feedback ---
With this script if the handwheel had been turned 3 times it would say `3 handwheel turned times`{:class='block3looks'}
  --- /feedback ---

- ( ) 
say (handwheel turned)
  --- feedback ---
With this script if the handwheel had been turned 3 times it would say `3`{:class='block3looks'}
  --- /feedback ---

--- /choices ---

--- /question ---
