## Who's in the puzzle room?

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
In this step you will add a character to a puzzle room, and create controls to move them around.
</div>
<div>
![](images/step_2.gif){:width="300px"}
</div>
</div>

--- task ---

Open [the Scratch starter project](https://scratch.mit.edu/projects/531567946/editor/){:target="_blank"}. Scratch will open in another browser tab. 

If you are working offline, you can download the starter project at [rpf.io/p/en/puzzle-room](https://rpf.io/p/en/puzzle-room).

[[[working-offline]]]

--- /task ---

You should see a scene from inside a spaceship. Several sprites have been made for you, and their positions have been set.

**Choose:** Who's in the spaceship? Is it just one character or is it a crew? It could be an alien spaceship or exist in a future where cats rule the world.

You can add as many characters as you like, but you need one character to interact with the puzzles you are making.

--- task ---

Add a new sprite to your project. In this example you will see the character Monet.

![animated gif of the Monet sprite from Scratch](images/monet.gif)

--- /task ---

If your character is too large or too small for the scene, then you should change its size. You can also pick a starting position for the character.

--- task ---

Add code to set up your character `when green flag clicked`{:class="block3events"}.

![monet sprite](images/monet-sprite.png)
```blocks3
when flag clicked
set size to (60) %
go to x: (0) y: (-130)
```

--- /task ---

You will need onscreen controls, to be able to move your character around.

--- task ---

Add an arrow sprite to your project. The sprite should have its mode set to `non draggable`{:class="block3sensing"} when the flag is clicked so it stays in place. When the sprite is clicked, it should broadcast the direction it is pointing so that it can control the character.

![arrow sprite](images/arrow-sprite.png)
```blocks3
when flag clicked
set drag mode [not draggable v]

when this sprite clicked
broadcast (right v)
```

--- /task ---

Now add more direction controls to move your main character.

--- task ---

Duplicate the arrow sprite three times. Then for each sprite, change the costume so it points in a different direction.

Change each sprite's name to the direction it is pointing and the `broadcast`{:class="block3events"} to the direction it is pointing

Arrange them all in the corner of the screen.

![the space scene with four arrows in the bottom left hand corner, pointing to the compass directions](images/arrows.png)

--- /task ---

Your main character should move when the arrows are pressed.

--- task ---

Code your main character sprite to move when it receives broadcasts to go `left, right, up and down`{:class="block3events"}.

![monet sprite](images/monet-sprite.png)
```blocks3
when I receive [up v]
change y by (10)

when I receive [down v]
change y by (-10)

when I receive [right v]
change x by (10)

when I receive [left v]
change x by (-10)
```
--- /task ---

--- task ---

**Test:** Click the green flag and then click on the arrows to move your character around.

--- /task ---


--- save ---
