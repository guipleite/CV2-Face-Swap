# Single image face swap using dlib and OpenCV
### Writen by:
- Eli Ghosn
- Guilherme Leite
- Rafael Rosenzvaig
### Professor Luciano Silva
### Insper - Computer Vision - 2020.2

___

The code presents an implementation for face swapping, between two different images, using two well-known computer vision python libraries: __dlib__ and __OpenCV__.

#### Implementation summary:
1. Load 2 images that contain a human face on it
2. Load pre-trained feature detection model
3. Apply model on images to retrieve features coordinates
4. Define facial area of interest using previously retrieved coordinates
5. Split facial area of interest into tringles
6. Cut facial region from both images and apply mask to remove the body from one image and the face from the other
7. Warp masked face image to allign with masked body image
8. Smooth edges to blend face into new body
9. Retrieve final image
