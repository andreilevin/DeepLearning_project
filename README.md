# **Teaching** **Neural** **Networks** to Play SET 

### Project Presentation [Slides](https://github.com/andreilevin/DL_project/blob/main/AndreiPresentation.pdf): 

[![AndreiPresentation.pdf:](https://raw.githubusercontent.com/andreilevin/DL_project/main/cover_screenshot.jpg)](https://github.com/andreilevin/DL_project/blob/main/AndreiPresentation.pdf)

## Summary

The goal of this deep learning project was to train neural networks to play the game SET  (rules explained [here](https://www.setgame.com/sites/default/files/instructions/SET%20INSTRUCTIONS%20-%20ENGLISH.pdf)) by recognizing the color, number, shading, and shape for each card in photograph of a 12-card hand.   To source my data, I took dozens of photos of  SET hands in different conditions (varying lighting, angle, background, etc.)  and used computer vision tools to extract an image of each individual card present.  After labeling and augmenting my image data, I used keras in tensorflow to train four different convolutional neural networks; one each to classify SET cards by shape, color, number, and shading.  Interestingly enough, while my color, shape, and shading classifiers achieved underwhelming test set accuracies of ~50-80%, my number classifier achieved a perfect 100% accuracy!  Thus, although I had initially set out to teach neural networks to play SET, in the end I only succeeded in teaching them how to count to three (I think [Joel Grus](https://joelgrus.com/2016/05/23/fizz-buzz-in-tensorflow/) would be proud).  On the plus side, my computer vision card extractor script worked exceedingly well— check out these perfectly  generated card borders in neon green:

<img src="https://raw.githubusercontent.com/andreilevin/DL_project/main/mvp_figs/fig4.png"  width="600" />  

## Tools
* OpenCV for card extraction 
* Pandas and OpenCV for labeling extracted cards
* Keras in Tensorflow for data augmentation and convnet modeling
