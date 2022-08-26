# unity-ar-face-detection

## unity version and packages
* unity 2021.3.2f1
* AR foundation
* AR-core XR Plugin (for android)

## build settings 
* switch platform to android

## project settings
* other settings > uncheck "auto graphics API" and remove "Vulkan"
* uncheck "multithreaded rendering"
* set "minimum API level" to API level 24
* set configuration > Scripting backend to "IL2CPP"
* Configuration > Target architectures check "ARM64" too

## scene setting
* delete camera
* H > XR > AR session Origin
* H > XR > AR session 
* AR Session Origin > add component -> AR Face Manager
* H > XR > AR Default Face
* Create New Material : Face Material and customise it (colour etc)
* AR Default Face > Mesh Renderer > Materials > drag our FaceMaterial
* Drag "AR Default Face" into PREFABS folder and delete it from H
* Drag "AR Default Face" into *AR Session Origin* > AR Face Manager (Script) > Face Prefab
* AR Session Origin > AR Camera > Ar Camera Manager component > Facing Direction > USER