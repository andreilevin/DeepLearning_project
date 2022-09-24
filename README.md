# **Teaching** **Neural** **Networks** to Play SET 

### Project Presentation [Slides](https://github.com/andreilevin/DL_project/blob/main/AndreiPresentation.pdf): 

[![AndreiPresentation.pdf:](https://raw.githubusercontent.com/andreilevin/DL_project/main/cover_screenshot.jpg)](https://github.com/andreilevin/DL_project/blob/main/AndreiPresentation.pdf)

## Summary

The goal of this project was to train neural networks to classify features of playing cards in the game SET (rules explained [here](https://www.setgame.com/sites/default/files/instructions/SET%20INSTRUCTIONS%20-%20ENGLISH.pdf)).   To source my data, I took 50+ photos of  SET hands in different conditions (varying lighting, angle, background, etc.)  and used computer vision tools to extract an image of each individual card present.  After labeling and augmenting my image data, I used keras in tensorflow to train convolutional neural networks to classify SET cards by shape, color, number, and shading.  Interestingly enough, while my color, shape, and shading classifiers only achieved test set accuracies of ~50-80%, my number classifier achieved a perfect 100% accuracy!  Thus, although I had initially set out to teach neural networks to play SET, in the end I only succeeded in teaching them to count to three (I think [Joel Grus](https://joelgrus.com/2016/05/23/fizz-buzz-in-tensorflow/) would have been proud).  On the plus side, my computer vision card extractor script worked exceedingly well— check out these perfectly  generated card borders:


<img src="https://raw.githubusercontent.com/andreilevin/DL_project/main/mvp_figs/fig4.png"  width="600" />  

