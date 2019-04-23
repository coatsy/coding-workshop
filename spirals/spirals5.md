# Adding Colour

[|< Home](../README.md)  
[<< Previous: Drawing a Spiral](./spirals4.md)  
[>> Next: More Challenges](./spirals6.md)

Up 'til now, the pen colour we've used has been whatever the standard colour is. It's time to jazz things up a bit.

## Cleaning Up

Every time you run the program, in addition to the spiral you're building, you get the two squares we made at the start. They've served their purpose and it's time for them to go.

Remember that whenever you drag a part of the program, all of the blocks underneath come as well so getting rid of the square drawing blocks is a 2-step process:

1. Drag them off the program
1. Put spiral loop bits back

Find the first `Move 100 steps` block - right after the `pen down` block and drag it just to the side of the program - still within the program pane. Don't worry if you make a mistake Ctrl+Z (on a PC) or Command+Z (on a Mac) will undo any mistakes you make.

![Move the square logic off the program](./images/clean-up-1.png)

Now pick up the spiral logic from the stack you just removed and reattach it to the program. Remember the spiral loop logic actually starts with the `set counter to 0` block that initialises the counter variable.

![Move the spiral logic back onto program](./images/clean-up-2.png)

Now when you run the program, just the spiral will appear.

![The spiral, unencumbered by squares](./images/clean-up-3.png)

[|< Home](../README.md)  
[<< Previous: Drawing a Spiral](./spirals4.md)  
[>> Next: More Challenges](./spirals6.md)
