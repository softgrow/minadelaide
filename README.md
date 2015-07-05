# minadelaide

Tools and scripts to transform 3DS data from the Adelaide City Council at https://data.sa.gov.au/data/dataset/3d-model into Minecraft worlds

# Usage
* Make sure you have the prerequsites, 200MB of free disk space, an internet connection and are aware of the limitations below
* Run the makeworld script and wait about 10 minutes to download and produce the objects around Rundle Mall
```
 $ ./makeworld
```

# Prerequesites
* [Blender](https://www.blender.org/) for transforming 3DS into Wavefront OBJ
* [Binvox 3D mesh voxelizer](http://www.cs.princeton.edu/~min/binvox/) for transforming Wavefront OBJ into Minecraft Schematics, Binvox uses the parity count method and (a slight variation of) the ray stabbing method described by Fakir Nooruddin and Greg Turk in Simplification and Repair of Polygonal Models Using Volumetric Techniques, GVU technical report 99-37 (later published in IEEE Trans. on Visualization and Computer Graphics, vol. 9, nr. 2, April 2003, pages 191-205)
* [MCEdit Unified](https://khroki.github.io/MCEdit-Unified/index.html) for inserting the schematics into Minecraft Worlds


# Limitations
* Only tested under OSX 10.10 and Minecraft 1.87
* Need to manually mirror each OBJ object in MCEdit before placing in a world
* Need to manually identify the largest dimension of each object in meters, some values used in the script may be incorrect
* Makes only individual objects, each object needs to be positioned relative to other objects in the Minecraft world Manually

Made with love, decaff, fizzy drinks, lollies and patience at Govhack 2015 (Unleashed Adelaide)
