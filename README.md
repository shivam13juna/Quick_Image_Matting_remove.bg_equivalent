# Quick Image Matting (remove.bg equivalent)
This repository shows a way for how to do image matting with precision similar to that of remove.bg

## Few steps to keep in mind
1. Mask is needed for performing image-matting, which can be obtained by <this repo>
2. Once we've a high quality mask, we can break down images and their corresponding masks into smaller slices and then use a function for estimating foreground and background, which we can just append with alpha and get the final image. 
3. Further, we parallelize the estimation part of foreground and background so that it gets the last percent of performance. With this method, we can perform image-matting of around 22 MP image in less than 20 seconds.  
  
  
  
Somehow getting mask through remove.bg, 

