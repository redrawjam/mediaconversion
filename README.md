# Conversion scripts
Google colab python scripts for image processing (vid to img + img to vid). To be use in conjuction with stable diffusions batch processing image to image functionality with controlnet. In order to convert simple video into animated diffusion style videos. Utilising cloud services by using google drive as the input and output directories.

## 🦒 Links to open the scripts in Colab.

| Colab Page | Function
| --- | --- |
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/redrawjam/mediaconversion/blob/main/Video_to_Image_Array_JRR.ipynb){:target="_blank"} | Video to image
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/redrawjam/mediaconversion/blob/main/Image_Array_to_Video_JRR.ipynb){:target="_blank"} | Image to video

## Tutorials
Video tutorials:
- Full conversion process (including stable diffuison control net conversion): https://www.youtube.com/
- Video to image usage: https://www.youtube.com/
- Image to video usage: https://www.youtube.com/

## Text tutorials:- Video to image usage:
1) Find or create a video in an mp4 format (using the .mp4 file extension).
2) Rename the video file to 'my_video.mp4'.
3) Place the video inside the video input directory in google drive. The directory is defined as the following by default: '/content/drive/MyDrive/conversion/videoconverter/videoinput/my_video.mp4'
---
![image](https://github.com/redrawjam/videotoimage/assets/34511774/7982c0b8-0e42-4af1-ae6e-e17ca54a65bc)
---
4) Run the Colab script.
---
![image](https://github.com/redrawjam/videotoimage/assets/34511774/64e6c13e-74d3-4ff3-b83d-96165dba3b67)
---
5) Confirm/ connect your google drive account.
---
![image](https://github.com/redrawjam/videotoimage/assets/34511774/0b62df44-55fa-45bc-b5d2-5a3252e50237)
---
6) Let it cook (takes a minute depending on the size of the video it is breaking down)
7) Check the output at the base of the Colab notebook script (should show the number of frames extracted and confirm where it was extracted to)
---
![image](https://github.com/redrawjam/videotoimage/assets/34511774/8de717c1-e6b7-4d57-b679-b6941fddef05)
![image](https://github.com/redrawjam/videotoimage/assets/34511774/33ea1b81-74ef-4e19-80d7-875b3631ea8f)
---

## Text tutorials:- Image to video usage
1) Ensure you have placed your image array a specified input directory on google drive. The directory is defined as the following by default: '/content/drive/MyDrive/conversion/imageconverter/imageinput/'
---
![image](https://github.com/redrawjam/videotoimage/assets/34511774/37d9f274-16e8-42c5-9878-6bd8f952890d)
--- 
2) Enter the number of frames being converted into a video (for the image to video script) into the script:
Here I have it set to 216 frames. Update that value as needed.
```py
#modify the range variable below to match the number of input frames
for i in range(216):
```
---
![image](https://github.com/redrawjam/videotoimage/assets/34511774/4157171c-16e5-4515-9a48-5db2f2315936)
![image](https://github.com/redrawjam/videotoimage/assets/34511774/ac1f5802-7c4a-49ec-9d2f-c8fd9562e07f)
---
3) Run the Colab script.
---
![image](https://github.com/redrawjam/videotoimage/assets/34511774/d1556fa0-f958-451e-bacf-4b8d0bb90f1d)
---
4) Confirm/ connect your google drive account.
---
![image](https://github.com/redrawjam/videotoimage/assets/34511774/0b62df44-55fa-45bc-b5d2-5a3252e50237)
---
5) Let it cook (this step can take some time, its essentially a waiting game, longer waits for more images and bigger images)
6) Check the output at the base of the Colab notebook script (should show the number of frames extracted and confirm where it was extracted to)
---
![image](https://github.com/redrawjam/videotoimage/assets/34511774/68c62c70-1cdb-42ab-9cf1-47523f711b4c)
![image](https://github.com/redrawjam/videotoimage/assets/34511774/b59b57a3-0d9e-4de8-a8bf-58d2eb52ac70)
---


## Important things to note: 

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
---
![image](https://github.com/redrawjam/videotoimage/assets/34511774/4157171c-16e5-4515-9a48-5db2f2315936)
![image](https://github.com/redrawjam/videotoimage/assets/34511774/ac1f5802-7c4a-49ec-9d2f-c8fd9562e07f)
---
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


