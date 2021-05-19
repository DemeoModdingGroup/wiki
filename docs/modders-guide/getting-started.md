**Warning**: This guide is unfinished.
# Getting Started
A simple modding guide for adding some; text to the lobby area.

???+ warning
    This guide will only cover how to mod the **PC/Steam** version of Demeo.

## Prerequisites 
This guide assumes you have a general understanding of how to write C# code and general knowledge of how to perform simple actions in your IDE of choice (Add References, Build a Project, etc.)
You will need to install Melon Loader v0.3.x, a guide is available in the [Installing Demeo Mods]() guide.


## Project setup

Your project should be a C# Class Library targeting .NET Framework v4.6.1.

Before we start writing code we need to reference `MelonLoader/MelonLoader.dll` and `demeo_Data/Managed/Unity.CoreModule.dll`, these are standard for any Demeo mod and are found in your Demeo install directory.

There are two more references needed specifically for this guide; `demeo_Data/Managed/Unity.UI.dll` and `demeo_Data/Managed/Unity.TextMeshPro.dll`. These will allow us to create text and adding it to the scene.

## Mod Metadata
The first bit of code we need to write is the assembly info for MelonLoader to detect our dll as a mod.

In your `AssemblyInfo.cs` file, add the following section:
```csharp
// Melon Loader
[assembly: MelonLoader.MelonInfo(typeof(MyDemeoMod.MyDemeoMod), "MyDemeoMod", "0.0.0", "Me!", "https://github.com/Me/MyDemeoMod")]
[assembly: MelonLoader.MelonGame("Resolution Games", "Demeo")]
```