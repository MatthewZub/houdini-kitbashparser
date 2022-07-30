# Description
<h4 align="center">
  'Kitbash Parser' is opensource kit of tools to work with kitbash packs in Houdini.
  
  Parser works and tested for Houdini 19.0, 18.5. So , it works for both python2 and python3 builds.
  
  <img src="https://user-images.githubusercontent.com/97801456/181500410-8caae4e7-94c3-4e9d-a4d8-49db2d2a0d51.png" width="500" >
  
</h4>


#### Suported Renders
- Mantra (Principled Shader)
- Mantra ([MRP Principled Shader](https://github.com/MainRoadPost/houdini_configs))
- Arnold (Standart Surface Shader)

<details>
     <summary>Supported\Tested Packs</summary>
     <p>
     
- [*Aftermath*](https://kitbash3d.com/products/aftermath)
- [*Anncient Temples*](https://kitbash3d.com/products/ancient-temples)
- Arch Vogue 
- City Streets
- Colonial
- Cyberpunk Minikit
- DMZ
- Dark Fantasy
- Elysium
- Every City
- Gaea
- Goliath
- Heavy Metal
- Outpost
- Los Angeles / DTLA
- Lunar Base
- Manhattan
- Medieval Marketplace
- Neo Dubai
- Savage
- Secret Lab
- Shangri La
- Soviet Blocks
- Space Colony
- Steampunk 
- Storefronts
- Treasure Island
- Valhalla
- Wasteland
- Wild West
- ~~Spaceships~~ - **DOES NOT WORK AT ALL**

</p>
</details>

# Installation

Just copy downloaded hda's to ``` <USER>/Documents/<HOUDINI_DIR>/otls/ ``` directory

# Usage

<h2 align="center">
  <img src="https://user-images.githubusercontent.com/97801456/181995823-e0cb84da-710b-4245-a4aa-f10d558c2b54.png" width="20">  KITBASH MAIN
</h2>

<img src="https://user-images.githubusercontent.com/97801456/181506255-8f0de960-e06b-41e9-90a8-92ba29ece2cd.png" width="700">

<img src="https://user-images.githubusercontent.com/97801456/181995910-7a007a94-d713-451f-b596-ae0a6cc06a7f.png" width="15">|
```Kitbash Folder``` - Select folder with your kitbash packs

<img src="https://user-images.githubusercontent.com/97801456/181995910-7a007a94-d713-451f-b596-ae0a6cc06a7f.png" width="15">|
```Format``` - Select the required format

<img src="https://user-images.githubusercontent.com/97801456/181995910-7a007a94-d713-451f-b596-ae0a6cc06a7f.png" width="15">|
```Load``` - ????

<img src="https://user-images.githubusercontent.com/97801456/181995910-7a007a94-d713-451f-b596-ae0a6cc06a7f.png" width="15">|
```Pack``` - The found packages will appear here

<img src="https://user-images.githubusercontent.com/97801456/181995910-7a007a94-d713-451f-b596-ae0a6cc06a7f.png" width="15">|
```Fix Rotation``` - Some of obj models are rotated due to different axis. So toggle it when the objects are rotated wrong

<h2 align="center">
  <img src="https://user-images.githubusercontent.com/97801456/181996409-bcf0521a-358b-49cc-a7a8-b9e3ff409e9e.png" width="20"> KITBASH MODEL
</h2>

<img src="https://user-images.githubusercontent.com/97801456/181511072-60184702-77c9-4e50-b8d1-aaef0dc6e9a1.png" width="700">

Wire input of this node to the output of ```KITBASH MAIN``` node

<img src="https://user-images.githubusercontent.com/97801456/181995910-7a007a94-d713-451f-b596-ae0a6cc06a7f.png" width="15">|
```Kitbash Model``` - After input wired , this menu will be filled with models names

<img src="https://user-images.githubusercontent.com/97801456/181995910-7a007a94-d713-451f-b596-ae0a6cc06a7f.png" width="15">|
```Color Per Material``` - Toggle parm just for undestanding how much materials

<img src="https://user-images.githubusercontent.com/97801456/181995910-7a007a94-d713-451f-b596-ae0a6cc06a7f.png" width="15">|
```Proxy``` - Toggle parm to switch from heavy model to simplify boxes

<img src="https://user-images.githubusercontent.com/97801456/181995910-7a007a94-d713-451f-b596-ae0a6cc06a7f.png" width="15">|
```Parsing Method``` - Menu , which appears only when you parsing OBJ file. You can choose method to parse that obj file.

<h2 align="center">
     <img src="https://user-images.githubusercontent.com/97801456/181996458-42feb530-44da-40ab-9528-3ff084d2fe45.png" width="20"> KITBASH SHADING
</h2>

<img src="https://user-images.githubusercontent.com/97801456/181512046-53b4222a-c8d9-4b8c-a0a5-d8b139ca15e3.png" width="700">

Wire output of this node to the input of ```KITBASH MAIN``` node

<img src="https://user-images.githubusercontent.com/97801456/181995910-7a007a94-d713-451f-b596-ae0a6cc06a7f.png" width="15">|
```Texture Folder``` - Еhe folder where the textures are located. This parameter using python to locate it self , but it works only if texture folder located in the same folder as geometry folder. If its not - select folder yourself :)

<img src="https://user-images.githubusercontent.com/97801456/181995910-7a007a94-d713-451f-b596-ae0a6cc06a7f.png" width="15">|
```Render Material``` - Select the render whose materials you want to create 

<img src="https://user-images.githubusercontent.com/97801456/181995910-7a007a94-d713-451f-b596-ae0a6cc06a7f.png" width="15">|
```Convert to acescg``` - Converting textures to acescg

<img src="https://user-images.githubusercontent.com/97801456/181995910-7a007a94-d713-451f-b596-ae0a6cc06a7f.png" width="15">|
```Build Materials``` - Create materials node inside. You can jump into and modify them

<img src="https://user-images.githubusercontent.com/97801456/181995910-7a007a94-d713-451f-b596-ae0a6cc06a7f.png" width="15">|
```OGL Textures``` - Enabling this parm will show you diffuse , roughness and normal textures in viewport. May cause lagging , cuz it is quite heavy 

<img src="https://user-images.githubusercontent.com/97801456/181995910-7a007a94-d713-451f-b596-ae0a6cc06a7f.png" width="15">|
```Shader Settings``` - Some of global texture settings

<h4 align="center">
  fetch_shaders.hda
</h4>

This asset is simply declaring materials if they were packed. So you no need to set 'Declare all shaders and materials' in Mantra ROP

# Features

- Custom shading networks
- Prefering Textures format
- Parsing textures via their names , without any mtl files

# Attributions

- Icon made by Freepik from [flaticon](www.flaticon.com)
- Icon made by Google from [flaticon](www.flaticon.com)
