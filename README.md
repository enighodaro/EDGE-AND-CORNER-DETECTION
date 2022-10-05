# EDGE-AND-CORNER-DETECTION
Implemented the Sobel filter, Canny edge detector, Harris corner detector

Sobel filter: It is used in image processing and computer vision, particularly within edge detection algorithms where it creates an image emphasising edges. It is based on convolving the image with a small, separable, and integer-valued filter in the horizontal and vertical directions and is therefore relatively inexpensive in terms of computations. On the other hand, the gradient approximation that it produces is relatively crude, in particular for high-frequency variations in the image. 

The Canny edge detection is a technique to extract useful structural information from different vision objects and dramatically reduce the amount of data to be processed. 
The process of Canny edge detection algorithm:
    Apply Gaussian filter to smooth the image in order to remove the noise
    Find the intensity gradients of the image
    Apply gradient magnitude thresholding or lower bound cut-off suppression to get rid of spurious response to edge detection
    Apply double threshold to determine potential edges
    Track edge by hysteresis: Finalize the detection of edges by suppressing all the other edges that are weak and not connected to strong edges.
    
Harris corner detector takes the differential of the corner score into account with reference to direction directly, instead of using shifting patches for every 45 degree angles, and has been proved to be more accurate in distinguishing between edges and corners.
The process of Harris corner detector algorithm:
      Color to grayscale
      Spatial derivative calculation
      Structure tensor setup
      Harris response calculation
      Non-maximum suppression
