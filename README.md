# SOM-neural-net



We need to design a Kohonen self organizing map (SOM), which gives as an output some shades of color mapped over
100 by 100 grid of neurones. The training input of the SOM are 24 colors (use shades of red, green, blue, with some
yellow, teal and pink) which you can chose from the "RGB Color Table: Basic Colors" section of this page:
http://www.rapidtables.com/web/color/RGB_Color.htm
Using a time varying learning rate 𝜶(𝒌) = 𝜶𝟎𝒆𝒙𝒑(−𝒌/𝑻) where k is the current training epoch (starts with
epoch 0), 𝜶𝟎 = 𝟎. 𝟖 , and T is the Total number of training epochs equal to 1000. Note that the epoch training
involves all twenty four input samples for the 24 chosen colors to the network (hint: calibrate the color codes
to values between 0 and 1, instead of being between 0 and 255). Initial weights are randomized. The
topological neighbourhood 𝑵𝒊,𝒋(𝒌) of node (j) around the winning unit (i) is given by

![image](https://github.com/Hediyeh-Safari/SOM-neural-net/assets/82396645/c514c87e-6885-43ec-b048-aba1279754cf)
where
![image](https://github.com/Hediyeh-Safari/SOM-neural-net/assets/82396645/16e08bdf-5294-4b37-855c-cb305db0bd1b)

And 𝑑𝒊,𝒋 is the distance between the winning node i and surrounding node j.
a) Generate a figure of the original grid (random weights) followed by figures of the SOM after 20, 40, 100, 1000
epochs. Change the value of 𝜎0 = 1, 10, 30, 50, 70.
b) Draw your conclusions on how the output changes with 𝜎0 and the number of epochs.
Note: Basically, we need to have as the output of the SOM colors similar to:
http://www.cs.hmc.edu/~kpang/nn/som.html (under “Demonstration”).


Reference use for this Question
http://www.cs.hmc.edu/~kpang/nn/som.html
