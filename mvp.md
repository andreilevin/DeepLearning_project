# Andrei's DL Project MVP

I'm working on a program that can play the game SET by recognizing the color, number, shading, and shape for each card in photograph of a 12-card hand.  To source my data, I took 56 photographs of seven 12-card hands such that each individual card is featured 8 times  (2 different surfaces x 2 different times of day x 2 different angles).

Using OpenCV, I wrote a program that identifies cards in each hand and extracts them into a square image, as shown below:

<img src="https://raw.githubusercontent.com/andreilevin/DL_project/main/mvp_figs/mvpfig1.png"  width="600" />

<img src="https://raw.githubusercontent.com/andreilevin/DL_project/main/mvp_figs/mvpfig2.png"  width="600" />

<img src="https://raw.githubusercontent.com/andreilevin/DL_project/main/mvp_figs/mvpfig3.png"  width="600" />

Now I need to figure out a way to:

(1) Save the 672 extracted card images as my training data and label the classes

(2) Figure out how much and what type of data augmentation to do (some obvious candidates are the four 90-degree rotations and blurring)

(3)  Train 4 individual neural networks (one on the full color images and three on grayscale images)

(4) ??

(5) Profit