# Detection of Moving Objects
Computer vision lightweight and fast detection of moving objects

## Introduction
Determination of moving objects is an important task of computer vision. <br>
Previously, many types of moving object detectors have been developed.  
Several approaches are generally used. The most simple one is to subtract  
adjacent subsequent frames of the video to extract changes that correspond to  
motion. While simple, such a detector has a disadvantage that only some spots  
of moving objects are detected. A more advanced approach is to separate the  
observation area into a quasistationary background and changing moving foreground.  
The next approach is to use optical flow computations to define moving objects.  
Finally, complex artificial neural networks are developed and trained nowadays  
to detect moving objects of interest.  
The present detector is based on separation of the frames into background and  
moving foreground. Since the algorithm uses very simple computations, the present  
detector is suitable for single-core computers and edge devices. 

## How it works
The background that constitutes a steady part of the movy is computed by averaging  
some number of the video frames. The background is dynamically updated by removing  
older frames and adding most recent ones. Moving objects areas are spotted via  
subtracting background from the current frame. There are several parameters that  
control the output of the detector including minimum moving object size and  
the minimum contrast. More about the parameters is described in the tuning section.  

## Installation 
  
  
## Usage  
  

## Tuning

