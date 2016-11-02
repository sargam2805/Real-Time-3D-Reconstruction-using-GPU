# Real-Time-3D-Reconstruction-using-GPU
Parallelize the serial implementation of 3D scene reconstruction with input from kinect sensor and run it on NvidiaGPU using CUDA.

This is the implementation of the paper Volumetric 3D Mapping in Real-Time by Frank Steinbrucker, et al

Include/install following libraries/software before running the code:

Glew

Glut

Eigen

QGLViewer

libQGLViewer-qt4

Boost

Opencv2

Qt 4

Glib

Valgrind & Kcachegrind

Steps to run the code:

1. Extract the folder  to desktop

2. cd  ~/Desktop/fastfusion

3. cmake . 

4. make

5. ./bin/onlinefusion ~/Desktop/fastfusion/rgbd_dataset_freiburg3_long_office_household/associate.txt --thread-fusion

6. Press “s” to start reconstruction

The time profiling is done using valgrind and you can open the file Desktop/fastfusion/callgrind.out.13830 using Kcachegrind to view the profiling done by us.

Refrences:

https://github.com/tum-vision/fastfusion

http://vision.in.tum.de/_media/spezial/bib/steinbruecker_etal_icra2014.pdf

http://vision.in.tum.de/data/datasets/rgbd-dataset/
