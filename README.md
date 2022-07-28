# Description
'Kitbash Parser' is a kit of tools to work with kitbash packs in Houdini.

Parser works and tested for Houdini 19.0, 18.5. So , it works for both python2 and python3 builds.

<img src="https://user-images.githubusercontent.com/97801456/181500410-8caae4e7-94c3-4e9d-a4d8-49db2d2a0d51.png" width="500" >

#### Suported Renders
- Mantra (Principled Shader)
- Mantra ([MRP Principled Shader](https://github.com/MainRoadPost/houdini_configs))
- Arnold (Standart Surface Shader)

#### Supported\Tested Packs
- Aftermath
- Anncient Temples 
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

# Installation

Just copy downloaded hda's to ``` <USER>/Documents/<HOUDINI_DIR>/otls/ ``` directory

# Usage

##### KITBASH MAIN
<img src="https://user-images.githubusercontent.com/97801456/181506255-8f0de960-e06b-41e9-90a8-92ba29ece2cd.png" width="700">

```Kitbash Folder``` - Select folder with your kitbash packs

```Format``` - Select the required format

```Load``` - ????

```Pack``` - The found packages will appear here

```Fix Rotation``` - Some of obj models are rotated due to different axis. So toggle it when the objects are rotated wrong

##### KITBASH MODEL
<img src="https://user-images.githubusercontent.com/97801456/181511072-60184702-77c9-4e50-b8d1-aaef0dc6e9a1.png" width="700">

Wire input of this node to the output of ```KITBASH MAIN``` node

```Kitbash Model``` - After input wired , this menu will be filled with models names

```Color Per Material``` - Toggle parm just for undestanding how much materials

```Proxy``` - Toggle parm to switch from heavy model to simplify boxes

```Parsing Method``` - Menu , which appears only when you parsing OBJ file. You can choose method to parse that obj file.
##### KITBASH SHADING
<img src="https://user-images.githubusercontent.com/97801456/181512046-53b4222a-c8d9-4b8c-a0a5-d8b139ca15e3.png" width="700">

Wire output of this node to the input of ```KITBASH MAIN``` node

```Texture Folder``` - Еhe folder where the textures are located. This parameter using python to locate it self , but it works only if texture folder located in the same folder as geometry folder. If its not - select folder yourself :)

```Render Material``` - Select the render whose materials you want to create 

```Convert to acescg``` - Converting textures to acescg

```Build Materials``` - Create materials node inside. You can jump into and modify them

```OGL Textures``` - Enabling this parm will show you diffuse , roughness and normal textures in viewport. May cause lagging , cuz it is quite heavy 

```Shader Settings``` - Some of global texture settings

##### fetch_shaders.hda
This asset is simply declaring materials if they were packed. So you no need to set 'Declare all shaders and materials' in Mantra ROP

# Attributions

- Icon made by Freepik from [flaticon](www.flaticon.com)
