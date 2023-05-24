# Conversion scripts
Google colab python scripts for image processing (vid to img + img to vid). To be use in conjuction with stable diffusions batch processing image to image functionality with controlnet. In order to convert simple video into animated diffusion style videos. Utilising cloud services by using google drive as the input and output directories.

## 🦒 Links to open the scripts in Colab.

| Colab Page | Function
| --- | --- |
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/18Yf4p23C5oXni98Gbdn7jz9Zx4eYq2aI?usp=sharing) | Video to image
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1h5QNzgCZfJDskGExA9F7n2ZH1l-lxdvf?usp=sharing) | Image to video

## Tutorials
Video tutorials:
- Full conversion process: https://www.youtube.com/
- Video to image usage: https://www.youtube.com/
- Image to video usage: https://www.youtube.com/


🚨 Important things to note: 

1) You need to ensure the video file you place in the input directory is titled 'My_video.mp4', as specified in the following line of code (for the video to image script):
```py
# Set up video path
video_path = '/content/drive/MyDrive/conversion/videoconverter/videoinput/my_video.mp4'
```
![image](https://github.com/redrawjam/videotoimage/assets/34511774/79c1f4da-347d-4fce-850c-8f171775e847)

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


