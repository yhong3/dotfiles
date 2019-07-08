# Unity mobile development
## build on Android 

https://unity3d.com/learn/tutorials/topics/mobile-touch/building-your-unity-game-android-device-testing

#### What error I saw
When I was using unity build from build setting (Ctrl+Alt+B) 
platform: Android
Build and Run
* Unable to list target platforms.Please make sure the android sdk path is ...
* Could not determine java version from '9.0.1' 
* Gradle build failed

#### What did I do until it builds
Some useful info here https://www.reddit.com/r/Unity3D/comments/77azfb/i_cant_get_unity_to_build_run_my_game/
1. Install Android Studio
2. In Android Studio, Install Sdk tools from settings if not installed 
3. In Unity, point SDK to C:\Users\<username>\AppData\Local\Android\Sdk
4. substitute original android sdk\tools folder to tools_r25.2.5-windows, so 
    * sdk\tools -> sdk\tools_r28
    * `<downloaded r25 tools folder>` -> sdk\tools
5. install jdk 8 and point JDK to JDK 8 folder in Unity
6. In `Unity > build setting`, change from `gradle` to `internal`


### Ramble
- Canvas size real time synced with game view
