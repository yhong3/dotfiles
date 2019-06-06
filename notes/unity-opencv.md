https://thomasmountainborn.com/2016/09/11/unity-and-opencv-part-one-install/

1. Download OpenCV (current 4.1.0), extract file to some temp folder
2. Download CMake, extract to some temp folder
3. Run CMake.exe
    - "Browse source" to opencv\sources
    - "Browse build" to some temp folder
    - "Configure" to choose installed visual studio version
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
