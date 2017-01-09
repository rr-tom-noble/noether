# 10.R8706

This package depends on PCL 1.8 and VTK 7.1.  Install VTK first and make sure that PCL is compiled against 7.1 or there will be run time errors.

VTK can be found here:
https://gitlab.kitware.com/vtk/vtk

PCL can be found here:
https://github.com/PointCloudLibrary/pcl

After building VTK and PCL, compile code using either catkin_make or catkin build (catkin tools).  To see examples, run the unit tests for each package:
catkin_make run_tests_<package-name>
e.g.: catkin_make run_tests_tool_path_planner

The noether package has an executable which is able to take in a mesh file (.stl format), read it, segment the file into adjacent surfaces,
and plan paths for each surface.  Work is in progress to read in point cloud (.pcd) files, but meshing results are not reliable right now.

