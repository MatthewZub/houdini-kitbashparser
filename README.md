# Description
'Kitbash Parser' is a kit of tools to work with kitbash packs in Houdini.

Parser works and tested for Houdini 19.0, 18.5. So , it works for both python2 and python3 builds.

<img src="https://user-images.githubusercontent.com/97801456/181500410-8caae4e7-94c3-4e9d-a4d8-49db2d2a0d51.png" width="350" height="300">

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

###### KITBASH MAIN
Create kitbash main node , select folder with kitbash models, choose format to parse and press 'Load"

Choose presented pack.

###### KITBASH MODEL
Create kitbash model node and wired input to the output of kitbash main node. After that in ordered menu of kitbash model node fill with models names

###### KITBASH SHADING
Create kitbash shading node and wired output to the input of kitbash main node. After that 

# Attributions

- Icon made by Freepik from [flaticon](www.flaticon.com)
