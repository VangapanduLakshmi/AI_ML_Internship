# AI_ML_Internship
step 1. Problem Statement:
Task: Separate the center area from images using perspective transformation.
Input: An image containing a rotated square or similar object.
Output: A cropped image with the center area isolated.

step 2. Step-by-Step Approach:
    Step 1: Load and Display the Image
      Use OpenCV (cv2) to load the image (image.png in your case).
      Display the original image to visualize the starting point.
   
   Step 2: Define the Four Corner Points of Square
      Identify the four corner points of the  square manually or programmatically.
      These points are crucial for calculating the perspective transformation.
   
Step 3: Define Destination Points for Perspective Transformation
      Determine the dimensions (width and height) of the output image.
      Define the destination points  where the transformed image will be mapped.
      
Step 4: Compute Perspective Transformation Matrix
       Use cv2.getPerspectiveTransform() to calculate the transformation matrix (M) based on step2 and step3

Step 5: Apply Perspective Transformation
       Use cv2.warpPerspective() to apply the transformation matrix (M) to the original image (image).
       
Step 6: Extract and Display the Center Area
        Once transformed, extract the center area from warped_image.
        Display the cropped center area to visualize the isolated region.
