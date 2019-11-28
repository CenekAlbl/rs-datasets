This dataset contains images from both RS camera and GS camera. The cameras were mounted ~3cm apart in a fixed rig, facing the same way. The images are captured in a synchronized manner using external trigger signal.

Calibration images as well as undistorted images included.

K matrices from OpenCV calibration:

RS camera:

2.58786383e+03 0.00000000e+00 1.56905241e+03
0.00000000e+00 2.58897738e+03 9.83084264e+02
0.00000000e+00 0.00000000e+00 1.00000000e+00

GS camera:

1.05596094e+03 0.00000000e+00 7.53077504e+02
0.00000000e+00 1.05617700e+03 5.27454485e+02
0.00000000e+00 0.00000000e+00 1.00000000e+00

Note that the colors are strange due to missing auto white balance.

The RS reqdout time per line is calculated as 1 / (FPS * (image height + 28)). In this case FPS was set to 30, eventhough the readout was externally triggered. I.e. the readout time per line was 1.60565e-05 s and for the entire image 0.032883 s.

The cameras were triggered approximately at 30FPS (up to the non-realtime OS precision). Some images in the sequence might be missing due to the cameras not providing the images in time for various reasons.


