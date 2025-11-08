# Finger Drawing with Hand Tracking

This project explores real time hand motion capture for free space drawing. The program observes the hand through a webcam feed and uses a common library for landmark recognition to identify the position of the index finger. When the hand remains open the fingertip acts as a contact point for drawing across a blank digital surface layered on top of the live camera output. When the hand closes the drawing motion pauses which allows more control and less visual noise. It is surprisingly intuitive once you try it and feels almost like moving a brush in the air.

The system relies on a popular hand landmark model together with a video processing toolkit. A short sequence of geometric checks decides whether the hand is open. After that the fingertip coordinates translate directly into drawing strokes with adjustable thickness and adjustable color. Even though the idea is simple the experience can feel expressive and lightly playful which makes it a useful small demonstration or teaching example.

## Requirements

* Python 3 installed
* A functional webcam
* The libraries listed in the requirements file

You can install everything in one go from the terminal inside the project folder by runnig:

pip install -r requirements.txt



## Running the program

Execute the script:
python3 finger_draw.py



If the camera is accessible a new window will appear. Move your hand within view and begin to draw.
## Controls
* Open the hand to draw
* Close the hand to stop drawing
* Press c to clear the drawing surface
* Press r for red g for green b for blue
* Press plus to enlarge the brush and minus to decrease it
* Press q to exit the application

## Notes
It may be helpful to experiment with lighting to obtain smoother detection. A small amount of ambient light usually gives the most stable tracking. You might also consider small adjustments in color and brush scale to suit your desired effect.
