## Advanced Lane Finding



Meets Specifications
Keen student,
Congratulations, you finally made it!
I can see you did read the suggestions and comments from the previous review and followed the required guidelines to adjust your work carefully. The work was attractive due to the great ideas implemented and the presentation of the write-up too was cool.:star:

On a personal note, I honestly must say this is quite a good implementation of the Advanced Lane finding project and we urge you to continue with this great desire for excellence as you study with us here at :udacious:dacity.:trophy:

Extra Material
Check out the following for more information on the subject matter.

Real-time Vision-Based Lane Detection with 1D Haar Wavelet Transform on Raspberry Pi
Lane Detection Techniques: A Review which describes a similar approach.
Lane Detection based on Contrast Analysis
Robust lane finding using advanced computer vision techniques: Mid project update
Writeup / README
The writeup / README should include a statement and supporting figures / images that explain how each rubric item was addressed, and specifically where in the code each step was handled.

The write-up includes explanations of the methods used and has supporting images to demonstrate how every rubric point was addressed. Great job!.

Camera Calibration
OpenCV functions or other methods were used to calculate the correct camera matrix and distortion coefficients using the calibration chessboard images provided in the repository (note these are 9x6 chessboard images, unlike the 8x6 images used in the lesson). The distortion matrix should be used to un-distort one of the calibration images provided as a demonstration that the calibration is correct. Example of undistorted calibration image is Included in the writeup (or saved to a folder).

Well done! You correctly used OpenCV functions like findChessboardCorners and calibrateCamera to calculate the correct camera matrix and distortion coefficients using the calibration chessboard images provided in the repository. And as shown below, the undistorted image is almost the same as the real one!

[![chessboard](https://udacity-reviews-uploads.s3.us-west-2.amazonaws.com/_attachments/55679/1545905629/1.png)]

Pipeline (test images)
Distortion correction that was calculated via camera calibration has been correctly applied to each image. An example of a distortion corrected image should be included in the writeup (or saved to a folder) and submitted with the project.

Great job applying the calculated distortion correction to the test images and also displaying the results.

Suggestions and Comments
To gain more knowledge about distortion correction and camera calibration, please refer to the links below:

Geometric Image Transformations
Camera Calibration
Calibrate fisheye lens using OpenCV — part 1
Python cv2.undistort() Examples

[![road](https://udacity-reviews-uploads.s3.us-west-2.amazonaws.com/_attachments/55679/1545905646/2.png)]

A method or combination of methods (i.e., color transforms, gradients) has been used to create a binary image containing likely lane pixels. There is no "ground truth" here, just visual verification that the pixels identified as part of the lane lines are, in fact, part of the lines. Example binary images should be included in the writeup (or saved to a folder) and submitted with the project.

OpenCV function or other method has been used to correctly rectify each image to a "birds-eye view". Transformed images should be included in the writeup (or saved to a folder) and submitted with the project.

Methods have been used to identify lane line pixels in the rectified binary image. The left and right line have been identified and fit with a curved functional form (e.g., spine or polynomial). Example images with line pixels identified and a fit overplotted should be included in the writeup (or saved to a folder) and submitted with the project.

Here the idea is to take the measurements of where the lane lines are and estimate how much the road is curving and where the vehicle is located with respect to the center of the lane. The radius of curvature may be given in meters assuming the curve of the road follows a circle. For the position of the vehicle, you may assume the camera is mounted at the center of the car and the deviation of the midpoint of the lane from the center of the image is the offset you're looking for. As with the polynomial fitting, convert from pixels to meters.

The fit from the rectified image has been warped back onto the original image and plotted to identify the lane boundaries. This should demonstrate that the lane boundaries were correctly identified. An example image with lanes, curvature, and position from center should be included in the writeup (or saved to a folder) and submitted with the project.

Good implementation and drawing of area to identify lane and following lane curvature.

Thank you for the updates to the work:thumbsup:
Pipeline (video)
The image processing pipeline that was established to find the lane lines in images successfully processes the video. The output here should be a new video where the lanes are identified in every frame, and outputs are generated regarding the radius of curvature of the lane and vehicle position within the lane. The pipeline should correctly map out curved lines and not fail when shadows or pavement color changes are present. The output video should be linked to in the writeup and/or saved and submitted with the project.

Excellent video output, result_project_video_2.mp4! The pipeline successfully identified the lane pixels in all frames of the project video and did not fail where shadows existed. This is commendable work and shows how much time and commitment was put into this project. Keep it up!:star:

[![road](https://udacity-reviews-uploads.s3.us-west-2.amazonaws.com/_attachments/55679/1545905832/1.png)]

Discussion
Discussion includes some consideration of problems/issues faced, what could be improved about their algorithm/pipeline, and what hypothetical cases would cause their pipeline to fail.

Great discussion here. You have correctly identified problems your pipeline can face and where it may fail.

Extra Material
One can try using deep learning techniques as alternative to Computer vision techniques used in the current implementation
Check out this link on Experiment Using Deep Learning to find Road Lane Lines to get a feel of what deep learning techniques can bring to lane finding.
One can use this awesome nvidia's end-to-end deep learning for Self driving cars.
For more math and theory about deep learning technique, follow this article from ford's engineers.

