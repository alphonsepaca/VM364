# Lesson Plan

## Terrain

Import Character.Controller Unity Package

Menu Bar > GameObject > 3D Object > Terrain

In Project Window, select Terrain

In Inspector Window > Transform Component

Position X = -512

Position Y = -20

Position Z = -512

In Inspector Window > Terrain (Script) Component > Settings (cog wheel)

Resolution

• Terrain Width = 1024

• Terrain Length = 1024

• Terrain Height = 200

SIn Inspector Window > Terrain (Script) Component > Paint Height Tool

• Height = 20

Flatten

In Inspector Window > Terrain (Script) Component > Raise / Lower Terrain

• Soft Brush

• Brush Size

• Opacity (displacement per stroke)

• Click for mountains and hills

• Shift + Click for valleys and canyons

In Project Window, drag Standard Assets/Character Controllers/First Person Controller to Hierarchy

Position X = 0

Position Y = 2

Position Z = 0

In Hierarchy Window, delete Main Camera (only one Audio Listener)

Menu Bar > GameObject > Light > Directional Light

Position X = 0

Position Y = 40

Position Z = 0

Rotation X = 40

Rotation Y = 300

Rotation Z = 180

Play Game

Stop Game

Spend time to sculpt terrain

In Hierarchy Window, select Terrain

In Inspector Window > Terrain (Script) Component > Settings (cog wheel)

• Export Raw...

• Save As My_Heightmap.raw in Assets

Launch Photoshop

Open My_Heightmap.raw

Modify and save

In Inspector Window > Terrain (Script) Component > Settings (cog wheel)

Import Raw... My_Heightmap.raw

Import Skybox Package

Menu Bar > Edit > Render Settings

In Inspector Window > Skybox Material > add Skybox Material from project window

In Project Window > Select the Skybox that you added

In Inspector Window > Selct Front (Notice where textures are located / notice how a skybox works)

Play

Stop

Menu Bar > Import Asset > Terrain Asset

Inspect Project Window > Terrain Assets

In Hierarchy Window, select Terrain

In Inspector Window > Terrain > Paint Texture > Edit Texture > Add Texture

• Texture = Grass & Rock

• Tile Size X/Y = 15

• Add

Play Game

Stop Game

Edit Texture > Add Textture > Add New Texture

• Tile Size X/Y = 30

In the Inspector Window > Select the new Texture

Paint terrain texture

Menu Bar > File > Save Scene As = My_Terrain_Scene

Custom Terrain Textures

Open Resources/Grass_Master.jpg in Photoshop

Select Rectangular Marquee Tool

Set Rectangular Marquee Tool to 512×512

Click on grass

Menu Bar > Edit > Copy

Menu Bar > File > New = My_Grass

Menu Bar > Edit > Paste

Duplicate Layer

Menu Bar > Filter > Other Offset = 256×256

Erase seams

Menu Bar > File > Save As = My_Terrain/Assets/Custom_Assets/Textures/My_Grass.jpg

Spend time to make Rock_Master.jpg tileable

Open and inspect Resources/Terrain_Textures in Preview

Drag Resources/Terrain_Textures to Project Window/Custom_Assets

Spend time to paint terrain textures

Play Game

Stop Game

Menu Bar > File > Save Scene









