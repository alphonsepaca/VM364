# Terrain Details

Open the project and scene you made for the Terrain Lesson in Lesson 2 

In Hierarchy Window, select Terrain

In Inspector > Terrain (Script) Component > Paint Details

Edit Detail > Add Grass Texture > Detail Texture = Grass

Paint Grass

Play Game

Simple polygon plane with alpha texture, will always face camera (billboard sprite)

Open Grass.psd in Photoshop (alpha channel)

###Detail Mesh

Menu Bar > Assets > Import New Asset >

Resources/Cobblestone_Terrain_Detail/Cobblestone_Color.jpg

Menu Bar > Assets > Import New Asset >

Resources/Cobblestone_Terrain_Detail/Cobblestone.fbx

In Project Window, select Cobblestone

In Inspector Window > Scale Factor = 1

Apply

In Project Window, select Material/Cobblestone_material

In Project Window, drag Cobblestone_Color.jpg to Inspector Window: Main Color (if needed)

In Hierarchy Window, select Terrain

In Inspector Window > Terrain (Script) Component > Paint Details > Edit Details > Add Detail Mesh
* Detail Mesh = Cobblestone
* Healthy Color = Light Grey
* Dry Color = Light Grey
* Render Mode = VertexLit
* Add

Paint details > Erase Grass (Shift Key)

Paint details > Cobblestone

Play Game

Stop Game

Select Cobblestone > Edit Detail > Edit
* Random Width = 50
* Random Height = 10
* Healthy Color = Dark Grey
* Dry Color = Dark Grey
* Add

Paint details

Play Game

Stop Game

Open Maya > Set Project in Unity Assets > Create Pyramid

In Inspector Window > Terrain (Script) Component > Paint Details > Edit Details > Add Detail Mesh
* Pyramid
* You may need to resize the pyramid

Menu Bar > File > Save Scene As = My_Terrain_Scene

Terrain Setting

In Hierarchy Window, select Terrain

In Inspector > Settings for the Terrain

Detail Distance (how far before its clipped)

Tree Distance (far clipping)

Billboard Start (facing image plane)

Wind Settings (notice that grass blows in the wind, but not trees)

Menu Bar > GameObject > 3D Object > Wind Zone

Directional (all trees) or Spherical (set size)

Terrain > Terrain (Script) Component > Edit Trees > Bending Factor = 10

Play Game

Stop Game

Menu Bar > File > Save Scene As = My_Terrain_Scene