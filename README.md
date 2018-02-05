# Object-Detection-with-SSD

Implemented in python using torch library.  Training data is required.

The heart of this program lies in the detect function in  takes in a frame, a trained neural network, and a transformation function as inputs.  For the purpose of this demonstration, an .mp4 file will be taken as an input and will be split up by frames, each frame being feed into the detect function one at a time.  
