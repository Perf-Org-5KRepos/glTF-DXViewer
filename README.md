# DirectX GLTF Viewer Sample
This project was motivated by a lack of sample code demonstrating the graphics API agnostic nature of the [glTF specification](https://www.google.com). The sample code is written using modern C++, DirectX 11 and the Universal Windows Platform (UWP) for the client application. The client application could have been written using any application development platform that supports DirectX 11 rendering. This sample is a port of the [Khronos PBR WebGL Sample](https://github.com/KhronosGroup/glTF-WebGL-PBR) and supports the same feature set.

![Main Sample App Screenshot](https://raw.github.com/peted70/dx-gltf-viewer/master/img/screenshot1.PNG)

The screenshot is showing the DamagedHelmet sample file  being rendered in the scene window, some controls to the right to adjust transforms and a Tree View control with the scene hierarchy.

# Features

* Physically Based Rendering (PBR)
* Buffer Management
* Specification Support
* Loader
* Environment Map
* Selective PBR Rendering

The selective PBR rendering allow you to turn on and off different parts of the PBR shader to provide a better understanding of the visual effect of each.

![Selective PBR Rendering](https://raw.github.com/peted70/dx-gltf-viewer/master/img/selective-rendering.png)

# Dependencies
* [boost-signals2](https://www.boost.org/doc/libs/1_67_0/doc/html/signals2.html) (header only observer/observable pattern)
* [Microsoft.glTF.cpp](https://www.nuget.org/packages/Microsoft.glTF.CPP/)

I used [vcpkg](https://github.com/Microsoft/vcpkg) for any source code dependencies and [Nuget](https://www.nuget.org/) and the Visual Studio integration to install binary dependencies. Neither of which are requirements.

# Building
This project can be built using Visual Studio 2017 Version 15.6.7 on Windows 10 Fall Creators Update (16299.0). I have also testd with version 15.7.1 but needed to add '/d2CoroOptsWorkaround' as in coroutines some variables may get optimised causing an access violation.

# Further Information
Please see this article for full details around features and coding for this sample.

# Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.