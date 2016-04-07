# FisheyeCorrection
Projects the Fisheye 180 Degree image. Fisheye to Rectilinear Projection

Fish Eye to Rectilinear Projection
Developed by Anubhav Rohatgi 6/04/2016

Shortcomings - >
There is some obvious barrel distortion which could have been minimized
by tuning radii correction parameter. The lines in the image are not straight.
If I change the multiplication factor "2.0" in xf and yf calculations
the lines do become stright but at the cost of image zooming in.
The result can further be enhanced if I would have applied interpolation.
Fisheye Image also requries Illumination Correction and Sharpening.
Taking lens parameters into account the distortion can further be corrected.



Dependancies 
1. OpenCV 3.1
2. C++14

Steps to Build & Run 
0. Do not forget to change the path to the image in the main.cpp
1. go to the directory
2. mkdir build
3. cd build
4. cmake ..
5. make -jn ->> substitute n for the number of jobs/cores
6. ./fisheye

