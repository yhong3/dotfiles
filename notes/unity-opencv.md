[Build opencv and hook to unity from scratch by Thomas Moutain](https://thomasmountainborn.com/2016/09/11/unity-and-opencv-part-one-install/)
And [a thread for it (find sample unit file here)](https://forum.unity.com/threads/tutorial-using-c-opencv-within-unity.459434/)

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
may show error: OpenCV(4.1.0) C:\temp\opencv-4.1.0\modules\imgproc\src\color.cpp:182: error: (-215:Assertion failed) !_src.empty() in function 'cv::cvtColor'
-> ffmpeg is not set up correctly [Source](https://stackoverflow.com/questions/42191058/opencv-python-installation-missing-ffmpeg-windows)
-> or... [the sample code just don't work](https://stackoverflow.com/questions/54104304/opencv-python-crashes-after-playing-a-video)

## TODO
1. Check if unity use x64 or x86 opencv
2. (optional) build for static? 
https://stackoverflow.com/questions/24096329/opencv-unity3d-integration
https://stackoverflow.com/questions/7583172/opencv-as-a-static-library-cmake-options
https://stackoverflow.com/questions/29740613/how-to-use-opencv-in-unity3d
https://www.youtube.com/watch?v=m-QPjO-2IkA


### helpful links
[OpenCV official tutorial](https://docs.opencv.org/3.0-beta/doc/py_tutorials/py_feature2d/py_features_meaning/py_features_meaning.html#features-meaning)

[official cascade classfier sample code](https://docs.opencv.org/2.4/doc/tutorials/objdetect/cascade_classifier/cascade_classifier.html)

[template matching](https://docs.opencv.org/trunk/d4/dc6/tutorial_py_template_matching.html)
[python image recognition bot](https://medium.com/@martin.lees/image-recognition-for-automation-with-python-711ac617b4e5)
