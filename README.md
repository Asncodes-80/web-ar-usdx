# Web AR USDs

Checking a super simple Apple `.usdx` 3D format, to showing
some 3D model inside of the Apple Safari web browser.

## Preface

### glTF/glb

glTF is a file format for three-dimensional scenes and models. A glTF file
uses one of two possible file extensions: `.gltf` or `.glb`. Both of them,
contain a lot of references like external binary and texture resources.

### USDX/USDA

Universal Scene Descriptor. 3D file format of Apple. It present in 2018 with iOS12.
It's like glTF. Mac designers can create their object with *Reality Composer*.

## General nature

From a button or link a website or Android/iOS app, launch a
native AR View (in Android native is `ARCore` and in iOS native is `ARKit`).

In Android, if Google Play Services for AR isn't present on the device, fall back
gracefully to showing the model in Scene Viewer-powered 3D mode.

### Android: 

- ar_preferred: Always starts in an AR viewer, and users can manually switch to a 3D
viewer. If Google Play Services for AR isn't present, gracefully falls back to starting
in the 3D viewer.
- 3d_preferred: Always starts in a 3D viewer, and users can manually switch to an AR viewer.
- 3d_only

## Android device platform

Android personally use ARCore kit for supporting AR in Android devices, at 
Android 7.0 or latest. Android 7.0 or (API Level 24). In Android devices it
will use *glTF* or *glb* 3D file format.

## iOS device platform

Android in most cases use ARKit for supporting AR in their devices. at iOS12
or latest version of that users can use this feature directly in any where of
iOS ecosystem. In iOS devices it will use *USDX* and *USDA* 3D file format.

## TODO

- Checking Android tag for ARCore[]

# References

- To checking your glb file, [Check me](https://arvr.google.com/scene-viewer-preview)
- To check full reference of Android, [Read me](https://developers.google.com/ar/develop/scene-viewer)
- glTF 3D model assets, [Check repo](https://github.com/KhronosGroup/glTF-Sample-Models)
