## The button puzzle

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
In this step you will add your first puzzle, which will be pushing the button a certain number of times.
</div>
<div>
![](images/step_3.gif){:width="300px"}
</div>
</div>

The button will need to be pushed 5 times for the puzzle to be completed. For this you will need a `variable`{:class="block3variables"} to store the number of pushed

--- task ---

Create a new `variable`{:class="block3variables"} and call it `button pressed`{:class="block3variables"}

--- /task ---

At the start of the game, `button pressed`{:class="block3variables"} should be `0`.

--- task ---
Add the following blocks to the button sprite

![button sprite](images/button-sprite.png)
```blocks3
when flag clicked
set drag mode [not draggable v]
set [button pressed v] to (0)
```
--- /task ---

A `repeat until`{:class="block3control"} block is a loop that keeps repeating until a certain condition is met. In this case, it will be until the button has been pressed `5` times.

--- task ---

Add a `repeat until`{:class="block3control"} loop, and set its condition to be when `button pressed`{:class="block3variables"} is `equal`{:class="block3operators"} to `5`.

![button sprite](images/button-sprite.png)
```blocks3
when flag clicked
set drag mode [not draggable v]
set [button pressed v] to (0)
+ repeat until <(button pressed) = (5)>
```
--- /task ---

You can use the `join`{:class="block3operators"} to `say`{:class="block3looks"} to the player how many times the button has been pressed.

--- task ---

Place a `join`{:class="block3operators"} inside another one. Then add in the text you want, and the `button pressed`{:class="block3variables"} variable, all inside a `say`{:class="block3looks"} block.

For example:

![button sprite](images/button-sprite.png)
```blocks3
when flag clicked
set drag mode [not draggable v]
set [button pressed v] to (0)
repeat until <(button pressed) = (5)>
+ say (join [button pressed] (join (button pressed) [times])
```
--- /task ---

As the loop will end when the button has been pressed `5` times, the last block in the script will then be run. This can tell the player that the task is complete.

--- task ---

Use a `say`{:class="block3looks"} block to tell the player the task has been complete.

![button sprite](images/button-sprite.png)
```blocks3
when flag clicked
set drag mode [not draggable v]
set [button pressed v] to (0)
repeat until <(button pressed) = (5)>
say (join [button pressed] (join (button pressed) [times])
+ say (task complete) for (2) seconds
```

--- /task ---

Now the player needs to be able to push the button. They should only be able to press it, when the character is close to the button though.

--- task ---

Add blocks to detect if the character is close to the button, when the button sprite is clicked.

![button sprite](images/button-sprite.png)
```blocks3
when this sprite clicked
if <(distance to (Monet v)) < (50)> then
else
```

--- /task ---

If the character is close, and the button is pressed, then the `button pressed`{:class="block3variables"} variable can be increased. If the character is not close, the puzzle should reset.

![button sprite](images/button-sprite.png)
```blocks3
when this sprite clicked
if <(distance to (Monet v)) < (50)> then
+ change [button pressed v] by (1)
else
+ set [button press v] to (0)
```

--- task ---

**Test:** Run your project and move the character close to the button. When you click on the button 5 times, the task should be complete.

--- /task ---

