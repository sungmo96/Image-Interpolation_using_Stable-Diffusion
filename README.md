# Image-Interpolation_using_Stable-Diffusion

This repository consists of a jupyter notebook file you can run on google colab to create your own interpolation clips/gifs



## Explanation

1. Using the CLIP-Interrogator, we first obtain adequate prompts that match the images as our input.
2. These prompts are then used to generate multiple images that would later be used to create a clip or a gif.
3. We use SLERP as our morphing/interpolation method to get better results that would prevent from sudden jumps from one image to another.




## How to Use

1. Upload images to a folder named my_images (which would be created under contents folder after running the code up to the setup).
2. For CLIP-interrogator, we highly recommend the prompt mode to be "classic" and saving the prompts into a csv as 'desc.csv' unless you want to solely test out the CLIP interrogator, in which case you can use "rename" for your output mode. Also since Stable Diffusion cannot convert tokens of length 77 or higher, we recommend setting maximum file length to 75 or lower.
3. Once that is done, run through the code blocks until "Generate Frames", where you will be asked to control interpolation steps and and number of inference steps as parameters. We recommend around 25 steps for inference steps since the quality of images do not differ much with further inference. For interpolation steps, the more the better, but usually somewhere around 25 to 40 found to be suffice to create good quality clips. 
4. And lastly, the last block of code would return a mp4 file that you can download. Good Luck!

