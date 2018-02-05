# Object-Detection-with-SSD

Implemented in python using torch library.  Training data is required but the network to be trainded can be found in ssd.py.  A file with serialized weights can be used instead of training the data.  This file with pre determined weights is ssd300_mAP_77.43_v2.pth.

The heart of this program lies in the detect function which can be found in object_detection_commented.py.  This function takes in a frame, a trained neural network, and a transformation function as inputs.  For the purpose of this demonstration, an .mp4 file will be feed through a video slicer with the help of the imageio libraries, which will split the video by frames, each frame being feed into the detect function one at a time.  The detection function will add rectangles around objects with a label description of the object.  Each of these new frams will be appened together to recreate the new video with all of the labels in each frame.
