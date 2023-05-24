# Conversion scripts
Google colab python scripts for image processing (vid to img + img to vid). To be use in conjuction with stable diffusions batch processing image to image functionality with controlnet. In order to convert simple video into animated diffusion style videos. Utilising cloud services by using google drive as the input and output directories.

## 🦒 Links to open the scripts in Colab.

| Colab Page | Function
| --- | --- |
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/18Yf4p23C5oXni98Gbdn7jz9Zx4eYq2aI?usp=sharing) | Video to image
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1h5QNzgCZfJDskGExA9F7n2ZH1l-lxdvf?usp=sharing) | Image to video

## Tutorials
Video tutorials:
- Full conversion process (including stable diffuison control net conversion): https://www.youtube.com/
- Video to image usage: https://www.youtube.com/
- Image to video usage: https://www.youtube.com/

Text tutorials:
- Video to image usage
- Image to video usage

🚨 Important things to note: 

1) You need to ensure the video file you place in the input directory is titled 'My_video.mp4', as specified in the following line of code (for the video to image script):
```py
# Set up video path
video_path = '/content/drive/MyDrive/conversion/videoconverter/videoinput/my_video.mp4'
```
![image](https://github.com/redrawjam/videotoimage/assets/34511774/4768ae5b-5cf9-463e-80f0-750e1a2fea52)

2) You need to ensure you enter the correct number of frames being converted into a video (for the image to video script):
Here I have it set to 216 frames. Update that value as needed.
```py
#modify the range variable below to match the number of input frames
for i in range(216):
```
![image](https://github.com/redrawjam/videotoimage/assets/34511774/4157171c-16e5-4515-9a48-5db2f2315936)
![image](https://github.com/redrawjam/videotoimage/assets/34511774/ac1f5802-7c4a-49ec-9d2f-c8fd9562e07f)

3) All the directories can be changed. Using the following code snippet as an example:
```py
# Set up video path
video_path = '/content/drive/MyDrive/conversion/videoconverter/videoinput/my_video.mp4'
```

Throughout all scripts a path is set. For usage with google drive the core component of the directory is `/content/drive/MyDrive/...` 
What follows after the initial conponent is up the the user (you). Here are some examples for video output directories:
1) `/content/drive/MyDrive/conversion/videoconverter/finalvideo/`
2) `/content/drive/MyDrive/conversion/videoconverter/bestvideo/`
4) `/content/drive/MyDrive/conversion/videos/`
5) `/content/drive/MyDrive/videos`
6) `/content/drive/MyDrive/edits`


