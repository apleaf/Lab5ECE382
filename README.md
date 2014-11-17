Lab5ECE382
==========

Required Functionality:
http://youtu.be/v1W9mqv_yLc


Lab5 Controlling Lights with remote


###Pre Lab
![alt text](http://i59.tinypic.com/2hgrayf.png)

![alt text](http://i59.tinypic.com/2zpmkrc.png)





##Achieving Required Functionality

To modify the code for the required functionality, I had to first change the start.h file to include the hex numbers for the buttons on the remote I was using.  These values are shown in the table above.  Note, we had to add a button for Zero. Next, I modified the main of the start.h file to toggle the lights depending on if the one button or two button was pressed on the remote.


##Debugging
Initially, I was unsure of what I needed to change in the pinChange method.  Erik explained to me how I needed to set the irPacket to the irPacket shifted bit wise and or that with either a 1 or 0 to get the new answer for the irPacket.  I added these in two if statements in the start.c file, but I was still not achieving requiered functionality.  After examining my code for a while, I realized that in my .c file, I had defined the buttons for my remote with incorrect hex values.  Once I fixed that, my program worked and pressing the 1 and two buttons on the remote turned the red and green lights on my MSP430 on and off. 

##Conclusion
I was very confused about what I was supposed to do for this lab initially.  After speaking with Erik and he explained the two if statements I needed to add, I finally understood what it was doing and felt like I really comprehended what was going on.  

Documentation: C2C Erik Thompson explained the two if statements i needed to add to the start.c file to alter the irPacket value.
