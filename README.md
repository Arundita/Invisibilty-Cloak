Harry Potter’s Invisibility Cloak with OpenCV

For every frame, converted the color from RGB to HSV and generated mask to detect red color.
To segment out the red part from each frame, performed cv2 morphology open and dilation on the mask part, created an inverted mask using cv2 bitwise_not and performed bitwise_and with the inverted mask.
Displayed the static background image pixels only for the masked region thus creating the ‘invisible’ affect.
