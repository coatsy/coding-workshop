# Drawing a Spiral

[|< Home](../README.md)  
[<< Previous: Drawing a Line](./spirals3.md)  
[>> Next: Adding Colour](./spirals5.md)

Spirals are a special kind of repeating pattern. Starting in the middle of the spiral, each line, or leg, gets a little bit longer so by the time the cat gets back, it's a little bit further away.

![Zoomed-in start of spiral](./images/zoomed-spiral.png)

## Variables

To make each leg a little longer each time the commands are repeated, we need a way of keeping track of how long it should be each time.

In computer terms, this is called a variable, because it varies over the life of the program.

Variables are defined and accessed through the Variables group of blocks. In the Variables group, click the `Make a Variable` button.

![Make a variable](./images/variables-1.png)

In the screen that pops up, call the variable `counter` and make it for this sprite only. Then click `OK`.

![Variable name and scope](./images/variables-2.png)

Now you've defined the variable, you need to give it an initial value. In this case we're going to start with a line that's 1 long and go up by 1 each time we loop through.

Drag the `Set counter to 0` block to the bottom of the program.

![Initialise the counter variable to 0](./images/variables-3.png)

Now we're ready to start the spiral loop. Drag a `Repeat 10 times` block from the control group to the bottom of the program and change `10` to `100` (you may need to scroll the program pane down a little to find the bottom of the program).

![Spiral loop control block](./images/spiral-loop-1.png)

Just like making a square, building a spiral is just doing two things over and over again, moving and turning. The only extra thing to do is change how far the movement should be.

Each time we go through the loop we want to move a little further, so each time we're going to change the value of counter by 1. There's a block fro that in the Variables group. Add that block inside the loop.

![Increment the counter each time through the loop](./images/spiral-loop-2.png)

Now we'll add the 2 standard things - move and turn. Add a `Move 10 steps` block and a `Turn right 15 degrees` block. Note that these are inside the loop, under the `change counter by 1` block.

Change the turn block to `90` degrees.

![Moving and turning inside the loop](./images/spiral-loop-3.png)

If you run the program now, you'll just get a little square, but if you make the leg length the value of the counter variable, the spiral magic appears.

To make the leg length use the counter variable's value, choose the Variable group and drag the `counter` block onto the region of the move block where the value's currently 10.

![Drag the counter variable onto the move block](./images/spiral-loop-4.png)

There's a trick to getting the variable block in the right place - the left edge of the block needs to line up with the left edge of the text area.

![Line up the left edges of the block and text area](./images/spiral-loop-5.png)

Run the program now and you should have a simple spiral in the middle of your screen.

![Yay! A spiral](./images/spiral-loop-6.png)

## Adding a twist

Spirals can look even cooler if they have a twist to them. If you get the cat to turn a little bit more or less than 90 degrees you get some pretty cool effects.

Try that now, change the turn value inside your spiral loop from 90 to 91 degrees. Run the program again and enjoy the twist.

![Spiral with a twist](./images/spiral-loop-7.png)

[|< Home](../README.md)  
[<< Previous: Drawing a Line](./spirals3.md)  
[>> Next: Adding Colour](./spirals5.md)