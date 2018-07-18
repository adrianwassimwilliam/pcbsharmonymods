﻿## Texture Replacer for PC Building Simulator
This is a mod that allows you to overwrite pretty much any texture in the game with your own. As an example it overwrites a few of the desktop icons with Windows 98 versions and it changes the Ryzen 7 1700 texture to a 486DX. 
See the Quick Start section below on how to make your texture replacements with this!

## Requirements
Requires FusioN.'s modloader for PCBS.

## Install
1. Extract everything in the archive to the main directory of PC Building Simulator, overwrite if necessary

## Compatibility
Should work with all other mods as long as the PCBS modloader is installed.

## Credits
FusioN. for his PCBS modloader ( https://www.youtube.com/channel/UCb8NrhEi7gWJzVt1eVC7IRQ )
The Harmony C# patching library ( https://github.com/pardeike/Harmony )

## Quick Start Texture/Sprite Patching
1. Open the PCBS_Data folder with AssetStudio ( https://github.com/Perfare/AssetStudio )
2. Search for the Texture you want to change
	2a. Select "Show Type" -> "Texture2D"
	2b. Go to the "Asset List" tab and search for your texture, examples to search for are "Ryzen 5" or "icon_"
	2c. Note down the texture name
3. Copy the new image you want to use into this folder, PNG or JPG works, for best results make it the same size as the original texture (AssetStudio shows width and height in the preview window)
4. Now depending on if the texture is for a part or for an icon/poster or other graphics in the game:
	4a. Part texture: Open "Parts Texture Replacer.conf" with a text editor and add a line <texture name>|<your new texture file> so as an example it will look like "Ryzen 5 Quad Core 1400|newCpu.png"
	4b. Icon/poster/image: Open "Sprite Texture Replacer.conf" with a text editor and add a line <texture name>|<your new texture file> so as an example it will look like "icon_email|myMail.jpg"
5. Start the game and try it out!