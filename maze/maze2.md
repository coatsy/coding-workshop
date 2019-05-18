# Adding your own controls

[|< Home](../README.md)  
[<< Previous: Standing on the shoulders of giants](./maze1.md)  
[>> Next: Connecting your BBC micro:bit](./maze3.md)

As a starting point, the MazeRunner game uses the keyboard arrow keys to move the ball. In this part of the tutorial you will examine the code used to do that and add your own code to also allow the use of the WSAD keys.

Examine the code that runs when the green flag is pressed - the blocks that live under the event block that looks like this:

![Green flag event block](./images/add-controls1.png)

The first two blocks reset the maze to the first backdrop in the list of backdrops and ensures that the ball is the correct colour.

![Set up the initial look of the game](./images/add-controls2.png)

## My Blocks

The next block is one you may not have seen. It's an example of what scratch calls `My Blocks`, in this case one called `BallToStart`.

![My first My Block](./images/add-controls3.png)

This block tells scratch to look for another set of blocks with that name and to run all of those blocks then come back and continue. In this case the code is very simple, it just moves the ball back to a starting position.

![The BallToStart My Block](./images/add-controls4.png)

Other programming languages call this type of block `functions` or `methods` and they're useful for a couple of reasons.

Firstly, they allow you to get a bunch of code out of the way so things are easier to read. Secondly, and probably more importantly, they allow you to define functionality that is used more than once, so rather than having to copy code or repeat it somehow, you can just call the MyBlock from wherever that bit of work needs to be done. Have a look and see if you can find somewhere else in the code where the `BallToStart` block is used.

### Creating a My Block

The last bit of setup the game does is to reset the speed, score and level to their initial values. When you look at all of the setup blocks together they look like this:

![The BallToStart My Block](./images/add-controls5.png)

This is a prime candidate to break out into a `My Block`. To do that, click on My Blocks in the block groups area:

![Click My Blocks](./images/add-controls6.png)

Now click the `Make a Block` button

![Click Make a Block](./images/add-controls7.png)

In the next screen, give your new block a name, like `SetupGame` and click the OK button.

![Name your block](./images/add-controls8.png)

Once you click OK, a new block header will appear in your code area:

![Define your new block's code here](./images/add-controls9.png)

Extract the setup steps from the main code by dragging them off the Green Flag event block and onto your new header block. Note that the rest of the code will come along for now - that's ok, we'll fix that in a moment.

![Drag the new block's code under the header](./images/add-controls10.png)

Next, find the `SetupGame` block (or whatever you called it) in the My Blocks area and drag it across to the Green Flag event block.

![Add a call to your new My Block](./images/add-controls11.png)

Now move the actual game code, that is everything inside the `forever` loop back under the `SetupGame` block.

![Put the main game blocks back into the main event block](./images/add-controls12.png)

Finally, if you want to, you can move the `SetupGame` definition across to be with the other `My Block` definitions. This isn't required, but it's often considered good practice to keep all your `My Block` definitions together.

Run the game and test that everything still runs just as it did before.

## Adding Controls

[|< Home](../README.md)  
[<< Previous: Standing on the shoulders of giants](./maze1.md)  
[>> Next: Connecting your BBC micro:bit](./maze3.md)