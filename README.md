# Poc_boul-lanta_generic_generator
the goal of this project it's to check if i am available to generate automatically a generic of emission like koh-lanta, 
When you have a lot of footage and you don't want to see all videos, you can make an app to do the generic.
For that I will probably use **Python**. (I hate this language, but it looks like to be born for that)

## first step Take a picture of your participants
with an library, and some input pictures i will prepare my app to do some facial recognisation
probably with **insightface** or **face_recognition**

## step 2 : take a picture of all the footage every O,5 sec 
maybe i will need to downgrade the quality of the videos or pictures. if I have 6 successive pictures of my participants I will note it in a Json doc like that : 
[
  {"candidat": "Marc", "start": "01:12.5", "end": "01:16.0", "cam": "Cam1"},
  {"candidat": "Julie", "start": "04:30.0", "end": "04:34.0", "cam": "Cam2"}
]

maybe i could add some notation about the video if the participant is near of the camera if the camera is mooving. 

For this step maybe use **opencv-python (cv2)** or **ffmpeg-python**

_if I use picture for recognation it's for optimisation. it's a first idea_

## Step 3: cut the correct moments and paste them

### Step4: add visual effect : like name with flame
