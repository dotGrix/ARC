<br />
<p align="center">
  <img src="http://2kmodz.com/2km-arc.png"/>
  <p align="center">
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Report Bug</a>
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Request Feature</a>
  </p>
</p>

## Table of Contents

* [About the Project](#2km-arc)
* [Usage](#export-decompressed-archive)
* [License](#license)
* [Contact](#contact)
* [Acknowledgements](#acknowledgements)

## 2KM ARC

<img src="https://i.imgur.com/F4KAijk.png"/>

On April 28, 2015 WWE 2K released WWE 2K15, which was the first PC release of a Wrestling game since 2002 (WWE RAW). Since that time a community has formed organically and we collectively made discoveries that which allow custom content for the game, from full wrestlers to even sound. In that same time, community members made several tools to make the process of modding easier and as imaginable it could be quite time consuming having to navigate each of those tools. 2KM Arc is a recursive IO tool designed to make the process of modding almost instantaneous while cutting back on the unnessesary workflow and the exorbitant amount of files that compact folders.

Here's how:
* One time click injection of singular files with two methods of compression OODLE & ZLIB.
* Open any archive and have it deserialize with moments, allowing you to peer deep into an archives contents.
* Utility tools that allow an end user to mass deserialize entire folders of archives.
* Preview window for textures inside archives, no more having to extract a file to see what it looks like.
* The injection process allows you to keep the game open while modding, without having the need to restart the game to see results.
* Create completely new 2K archives from scratch.
* Drag 'n' Drop files. 

## Support Me
I work on Arc in my free time, this is a passion project. If you wish to support me and my efforts to make this tool better, you are welcome to send a donation. 

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XNPMKZG77WUCJ&source=url)
<br />

# General

## Export Decompressed Archive
Arc will extract the deserialized archive if it exists, if a decompressed version does not exist it will give you the compressed version and ultimately fail if neither exist in the context.

## Export Compressed Archive
Arc will extract the raw compressed archive if it exists. Arc will alert you if the archive does not exist.

<br />

# Import Compressed Archive

## ZLIB
With an archive node selected in the tree view that you wish to replace, this will ask for a new archive (e.g. PAC, Texture Archive, muscle file, masking file etc). Once chosen it will compress the archive with ZLIB (slower) then inject and replace the pre-existing archive. This can work on singular texture files.

## OODLE
With an archive node selected in the tree view that you wish to replace, this will ask for a new archive (e.g. PAC, Texture Archive, muscle file, masking file etc). Once chosen it will compress the archive with OODLE (Kraken) (very fast!) then inject and replace the pre-existing archive. This can work on singular texture files.

# Import Standard Archive

## SHDC
With a container node selected, this will ask for a new container such as BPE, PACH or SHDC. Once chosen, it will inject and replace the previous container with the new file.

## BIN
With a node selected, this will ask for raw binary you wish to replace the selected node with. Once chosen, it will inject and replace the previous archive file with the new   one. This can be equated to importing an uncompressed archive.

<br />

# Create (Toolbar)

## Texture Archive
Allows you to multi-select .DDS files and save them into a texture archive. This is useful for when creating new 000A and 000C archives.

## EPK8 Archive
Allows you to multi-select archives and save them into an EPK8 container - options to set the container name and type. These archives are especially unique and allow for greater control with 2K modding. 

## Container
Allows you to multi-select archives and turn them into either a SHDC or PACH container. SHDC/PACH containers are used in conjunction with HSPC and EPK8 containers. 

<br /><br />

# Utility (Toolbar)

## Mass Extract Directory
Pressing will open the first window asking where you would like to save the extracted containers/archives. The second window will ask where the files you're wanting to extract are located. Once this process has completed ARC will begin to deserialize and dump out the contents from the files you targetted. 

<br />

# Utility (Context Menu)

## Rename Header
Selecting a valid container or binary archive, this will open a new window with your object data. From here this allows you to rename/modify the pre-existing archive. This is useful when modding with EPK8 archives.

## Extract Texture(s)
With a binary archive selected that has the name '0014', this will prompt you for two locations. The first location is where you wish to store the extracted textures, and the second is the tx archive that contains the textures. Arc will then uncompress, convert and extract the textures to your chosen location.

## Sync Muscles
YOBJ file(s) have this utility available. When pressed, a window will appear asking you for the muscle archive (00CA) that belongs to the targetted YOBJ. Upon selecting the 00CA, ARC will use the pre-existing 00CA in the container and merge the muscle information onto the selected YOBJ and then inject back into the container. 

<br />

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact

Grix - [@dotGrix](https://twitter.com/dotGrix)


## Acknowledgements
* PerfectPlex (Imp)
* 2KM Discord/Community 
* Tekken57
* Xentax
* Keshire


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=flat-square
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=flat-square
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=flat-square
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=flat-square
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=flat-square
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
