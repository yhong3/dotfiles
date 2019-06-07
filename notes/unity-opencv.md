https://thomasmountainborn.com/2016/09/11/unity-and-opencv-part-one-install/

1. Download OpenCV (current 4.1.0), extract file to some temp folder
2. Download CMake, extract to some temp folder
3. Run CMake.exe
    - "Browse source" to opencv\sources
    - "Browse build" to some temp folder
    - "Configure" to
        1. choose installed visual studio version (e.g. Visual studio 15 2017),
        2. **Optional platform for generator** = x64 for 64bit, default was Win32 
    - "Generate" to build

If failed with 
``` 
Visual Studio 15 2017
could not find any instance of Visual Studio.
```
Then [Link](https://stackoverflow.com/questions/51668676/cmake-visual-studio-15-2017-could-not-find-any-instance-of-visual-studio)
```
Open Visual Studio
Go to Tools -> Get Tools and Features
In the "Workloads" tab enable "Desktop development with C++"
Click Modify at the bottom right
```
4. Open "opencv.sln" in the build folder, let it scan for a while, wait until it said "Ready"
5. find "INSTALL", right-click and "Set as a Startup project"




opencv-python
problem on loading avi file using cap = cv2.VideoCapture('vtest.avi')
-> ffmpeg is not set up correctly [Source](https://stackoverflow.com/questions/42191058/opencv-python-installation-missing-ffmpeg-windows)

## TODO
1. Check if unity use x64 or x86 opencv
2. (optional) build for static? 
https://stackoverflow.com/questions/24096329/opencv-unity3d-integration
https://stackoverflow.com/questions/7583172/opencv-as-a-static-library-cmake-options
https://stackoverflow.com/questions/29740613/how-to-use-opencv-in-unity3d
https://www.youtube.com/watch?v=m-QPjO-2IkA
