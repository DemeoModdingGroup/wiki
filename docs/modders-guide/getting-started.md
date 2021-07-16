**Warning**: This guide is unfinished.
# Getting Started
A simple modding guide for adding some; text to the lobby area.

???+ warning
    Only the PC/Steam edition of Demeo will be covered in this guide.

## Prerequisites 
This guide assumes you have a basic understanding of C# programming and a basic understanding of how to use your preferred IDE to perform simple tasks (Add References, Build a Project, etc.) Melon Loader v0.3.x must be installed; instructions can be found in the Installing Demeo Mods guide.

## Project setup

Your project should be a C# Class Library targeting .NET Framework v4.6.1.

Before we start writing code we need to reference `MelonLoader/MelonLoader.dll` and `demeo_Data/Managed/Unity.CoreModule.dll`, these are standard for any Demeo mod and are found in your Demeo install directory.

This guide needs two additional references: `demeo_Data/Managed/Unity.UI.dll` and `demeo Data/Managed/Unity.TextMeshPro.dll`. We'll be able to generate text and connect it to the scene using these.

## Mod Metadata
The assembly information that MelonLoader needs to recognise our dll as a mod is the first piece of code we need to write.
 
Add the following section to your `AssemblyInfo.cs` file:
```csharp
// Melon Loader
[assembly: MelonLoader.MelonInfo(typeof(MyDemeoMod.MyDemeoMod), "MyDemeoMod", "0.0.0", "Me!", "https://github.com/Me/MyDemeoMod")]
[assembly: MelonLoader.MelonGame("Resolution Games", "Demeo")]
[assembly: MelonPlatform(MelonPlatformAttribute.CompatiblePlatforms.WINDOWS_X64)]
```