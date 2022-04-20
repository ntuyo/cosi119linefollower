# cosi119linefollower
### By Nazari Tuyo

## The Code
The line follower code works as following: 
    1. the init method:
    * creates the bridge, which helps establish / simplify computer vision (from the camera) for the node
    * creates a subscriber and publisher for image_raw/compressed and cmd_vel respectively
    2. the image callback method:
    * this gets the image from the camera, storing it in an variable called 'image'
    * using cv2, the non-yellow colors in the frame are cut out
    * the remaining is masked out, so only yellow is visible
    * then a red circle is placed on the center of the line so the follower can continue moving

## Video
