# Andrei's Deep Learning Project Proposal

My goal is to code up a program that can help you play (or cheat at, depending on your moral compass) the card game SET (rules explained [here](https://www.ultraboardgames.com/set/game-rules.php) ).   In the final version, the user will upload an image like the one below and my program will identify any "Sets" present:

<img src="https://www.theboardgamefamily.com/wp-content/uploads/2013/03/SetCards2.jpg" alt="Set - card game of quick visual perception - The Board Game Family"  width="600" />

To do this, I will ideally need the following four ingredients:

1. An "object identifier" script that will accept a photo as input and identify and extract all the cards present in the photo.

2. A "card classifier" script that will accept an extracted card image as input and will tag it as one of the 81 possible set cards.
3. A "Set solver" script that will accept a list of classified cards and identify which triplets (if any) comprise a Set.
4. A "Set tagger" script which will go back and visually tag any sets in the original image (perhaps with bounding boxes?)  and return the tagged image as the final output.

Parts 1 and 4 can be tackled with traditional computer vision tools (I will use OpenCV).  For part 3 I'll write an algorithm in python.   The hardest part, and the only one requiring neural nets, will be part 2.  I plan to train 4 separate neural nets, one for each ternary card feature (color, number, shape, and shading) on a dataset of all 81 cards separately photographed.  I will also need to use data augmentation in Keras to increase the size of the training data set and make it more robust to changes in lighting, orientation, etc..  

A reasonable MVP could involve finishing part 1 and training one of the 4 neural nets used in part 2.  

In the best case scenario for the final project, I would build out a Streamlit app (note: the feasability of this will likely depend on how long my Thanksgiving turkey coma lasts) 

