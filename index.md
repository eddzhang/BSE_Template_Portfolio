# Object Detection With Raspberry Pi
This will serve as a brief description of your project. Limit this to three sentences because it can become overly long at that point. This copy should draw the user in and make she/him want to read more.

   | **Engineer** | **School** | **Area of Interest** | **Grade** |
   |:--:|:--:|:--:|:--:|
   | Eddie Zhang | Bellarmine College Preparatory | Electrical Engineering | Rising Junior


![Headstone Image](https://howchoo.com/media/ot/zk/zg/the-raspberry-pi-and-opencv-logos.png?width=900&auto=webp&quality=70)
  
[![List of Materials](https://docs.google.com/document/d/1v1GPGEsMnRYpzOPJANB8pGmUEhGZuY_O6Z3P3sVSDW8/edit?usp=sharing)

# Demo Night Presentation
[![Demo Night](https://res.cloudinary.com/marcomontalbano/image/upload/v1626121814/video_to_markdown/images/youtube--x-eQbkiBERM-c05b58ac6eb4c4700831b2b3070cd403.jpg)](https://www.youtube.com/watch?v=x-eQbkiBERM "Demo Night")


# Final Milestone
My final milestone is the increased reliability and accuracy of my robot. I ameliorated the sagging and fixed the reliability of the finger. As discussed in my second milestone, the arm sags because of weight. I put in a block of wood at the base to hold up the upper arm; this has reverberating positive effects throughout the arm. I also realized that the forearm was getting disconnected from the elbow servo’s horn because of the weight stress on the joint. Now, I make sure to constantly tighten the screws at that joint. 

[![Final Milestone](https://res.cloudinary.com/marcomontalbano/image/upload/v1612573869/video_to_markdown/images/youtube--F7M7imOVGug-c05b58ac6eb4c4700831b2b3070cd403.jpg )](https://www.youtube.com/watch?v=F7M7imOVGug&feature=emb_logo "Final Milestone"){:target="_blank" rel="noopener"}

# Second Milestone

For my second milestone, I installed OpenCV onto my Raspberry Pi in order to take photos and save photos. Then I wrote a function in python called apiCall() that sends the frame to my Nanonets model and it returns a JSON file. In the while loop, the code extracts the coordinate information from the JSON file and draws the box onto the frame. Finally, the code opens the image so that it is visible on the monitor. A difficulty I faces was debugging the python script. I was not familiar with the OpenCV commands so I had to search up their parameters. Reading a JSON file was also a new concept that was a bit confusing at first.

<p align="center">
  | Below are some important parts of my code |
</p>

This function sends a frame called "frame.jpg" to the Nanonets website and returns a JSON file with the coordinates of the boxes.
![image](https://user-images.githubusercontent.com/86021700/124323627-7bffa300-db36-11eb-83c2-e7c726d2b828.png)

This while loop reads the JSON file that is sent back from the Nanonets website and draws the boxes on the frame.
![image](https://user-images.githubusercontent.com/86021700/124323006-5cb44600-db35-11eb-89f2-4b211c709514.png)




# First Milestone
  
My first milestone was being able to set up the Raspberry Pi with the camera and sent my dataset of images and annotations into Nanonets in order to train a model. After training and retraining my model, I ended up with a model with 86% accuracy. A problem that I faced was when the Nanonets website declined my annotations. This was because the coordinates in the annotations were floats, which meant they had decimals. Since Nanonets does not read coordinates as decimals, my intrustor helped me redo the annotations so that the coordinates were integers.

[![First Milestone](https://res.cloudinary.com/marcomontalbano/image/upload/v1626121520/video_to_markdown/images/youtube--6DpmbO4qvxA-c05b58ac6eb4c4700831b2b3070cd403.jpg)](https://www.youtube.com/watch?v=6DpmbO4qvxA "First Milestone")

