# Quick Image Matting (remove.bg equivalent)
This repository shows a way for how to do image matting with precision similar to that of remove.bg

PS: You need this library for performing image extraction ![library](https://github.com/99991/matting)

# Key point of how to do it, is to get a good mask using any of the libraries like mask_gen, then use these steps:
1. Divide the images into multiple parts, in my case i've divided it in 9 parts. 
2. Estimate foreground combine it with alpha
3. Re-join all the images. 

In the notebook I demonstrate how to do above steps, assuming we've a mask


Example, 

![original image](<original_big.jpg>)

![mask of image](<conv_mask.png>)

![output from code](<finally.png>)



