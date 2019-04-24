# Flappy Bird

## Bird and gravity

First step is to make the bird, is to resize it to 60 so that it is not so big.

![resizeing of cat](./images/cat-resizing.png)

Now we need to give the cat gravity. We will do this by adding a when stat flag is clicked and setting a new variable called velocity to 3.

![velocity](./images/velocity.png)

You will se when you push the green flag that nothing happens. That is because the varible velocity is not being used anywhere. So lets add a change y by tab under neath and put velocity in it.

![changey-by-velocity](./images/changey-by-velocity.png)

You will see when you push the green button the cat move a small amount then stops and the cat move in the wrong direction. That is because the move function is only run once. Lets fix this by putting the change y by into a forever function and change the velocity to -3 so that this function is run forever and goes the opposite direction.

![correct-gravity](./images/correct-gravity.png)