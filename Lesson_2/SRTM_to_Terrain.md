# SRTM to Unity Terrain

Note: I still have not figured out how to create the height to scale. I also need to figure out how to stitch multiple .hgt files together.

In Google Maps find desired location:

Right Click > What's Here? > Get GPS coordinates

Go to [SRTM Database](http://dds.cr.usgs.gov/srtm/version2_1/SRTM3/)

Select Continent > GPS coordinate Zip > Download Zip > UnZip

Change extension from .hgt to .raw so that the file can be opened in photoshop.

Right Click .raw file and open with photoshop.

Settings:
* Width: 1201 pixels
* Height: 1201 pixels
* Count: 2
* Interleaved
* 8 Bits

Menu Bar > Image > Mode > Grayscale

Channels > Delete Gray Channel - Keep Alpha Channel

Menu Bar > Image Mode > Grayscale & 16 Bit (the Alpha channel should now be Gray) n

Channels > Double Click on Background to turn it into Layer 0

Adjustments > Levels > Adjust settings to get optimal gray details (For Boston: Top Slider: 0,2,80  OutPut Levels: 30 255)

Merge Layers

Select all & Copy

Menu Bar > File > New

Settings:
* Width: 1024 pixels
* Height: 1024 pixels
* Resolution: 72 pixels/Inch
* Color mode: Grayscale / 16 Bit
* Background Contents: Transparent
* Advanced: Color Profile: Gray Gamma 2.2 (Dot outputs are normally for print)
* Advanced: Pixel Aspect Ratio: Square Pixels

Paste .raw image

Convert Colors OK

Command T to resize image to canvas (use shift key)

File > Save As > Photoshop Raw file

IN UNITY

Menu Bar > Game Object > 3D Object > Terrain

Select Terrain in the Hierarchy View

Inspector > Terrain (Script) Component > Terrain Settings

Resolution:
* Terrain Width: 1201
* Terrain Length: 1201
* Terrain Height: 200 (What is the correct height for scale here?)
* Heightmap Resolution: 1025 (photoshop file resolution +1)

Import Raw > Select your .Raw file

Settings:
* Depth: 16 Bit
* Width: 1024
* Height: 1024
* Terrain Size: x = 1201  y = 200  z = 1201
* Import

Add RotateTerrain Script to Assets

Add RotateTerrain Script as Component on Terrain

Press Play

Adjust Terrain Resolution Height to 20:
* Terrain Height: 20 (What is the correct height for scale here?)






