# Image-Interpolation_using_Stable-Diffusion

This repository consists of a jupyter notebook file you can run on google colab to create your own interpolation clips/gifs



## Explanation

1. Using the CLIP-Interrogator, we first obtain adequate prompts that match the images as our input.
2. These prompts are then used to generate multiple images that would later be used to create a clip or a gif.
3. We use SLERP as our morphing/interpolation method to get better results that would prevent from sudden jumps from one image to another.




## How to Use

1. Upload images to a folder named my_images (which would be created under contents folder after running the code up to the setup).
2. For CLIP-interrogator, we highly recommend the prompt mode to be "classic" and saving the prompts into a csv as 'desc.csv' unless you want to solely test out the CLIP interrogator, in which case you can use "rename" for your output mode. Also since Stable Diffusion cannot convert tokens of length 77 or higher, we recommend setting maximum file length to 75 or lower.
![스크린샷(8)](https://user-images.githubusercontent.com/65227427/228434732-aa46cbd5-9dd2-46c8-9c5d-23e9acc5cd66.png)
![스크린샷(4)](https://user-images.githubusercontent.com/65227427/228434837-0fd60ef0-6b91-4bfb-8845-3a24c6ca00e5.png)


3. Once that is done, run through the code blocks until "Generate Frames", where you will be asked to control interpolation steps and and number of inference steps as parameters. We recommend around 25 steps for inference steps since the quality of images do not differ much with further inference. For interpolation steps, the more the better, but usually somewhere around 25 to 40 found to be suffice to create good quality clips. 
![스크린샷(7)](https://user-images.githubusercontent.com/65227427/228434767-cba466e2-adc2-4718-a6a0-0ff562bf7c6b.png)


4. And lastly, the last block of code would return a mp4 file that you can download. Good Luck!



## Images used and final results

- Images
![barren field](https://user-images.githubusercontent.com/65227427/228435040-ae08ffbf-28a3-4113-9069-c198623c8914.jpg)
![colonialamerica](https://user-images.githubusercontent.com/65227427/228435052-72125852-00dd-459a-88a2-b6974c6463ed.jpg)
![america1900s](https://user-images.githubusercontent.com/65227427/228435060-469211b2-f847-4e72-9958-e02104ee9712.jpg)
![capitol](https://user-images.githubusercontent.com/65227427/228435068-a195a41f-c47e-4fe2-b7d6-7be679c8f5bd.jpg)


- Final result

https://user-images.githubusercontent.com/65227427/228435182-a3f8d97e-d578-43ca-8178-fa09678d9c04.mp4


