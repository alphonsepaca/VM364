#Baking Lights

Open the project and scene you made for the Terrain Lesson in Lesson 2 

Menubar > Assets > Import New Asset = Resources/Crate/Crate_Color.jpg

Menubar > Assets > Import New Asset = Resources/Crate/Crate_Normal.jpg

Menubar > Assets > Import New Asset = Resources/Crate/Crate.fbx

In Project Window, select Materials/Crate_Color
Shader Pulldown Menu Bumped Diffuse
Add Crate_Normal to Normalmap
Fix Now
In Project Window, select Crate_Normal
In Inspector Window, √ Create from Greyscale
Bumpiness = 0.025
Apply
Insatiate Crate a few times in clearing with open light
In Hierarchy Window, select Directional Light
In Inspector > Light > Shadow Type = Soft Shadows
Lightmapping
In Hierarchy, select Create
In Inspector, √ Static
In Hierarchy, select Terrain
In Inspector, √ Static
Menubar > Window > Lightmaping >
Lightmap Size = 1024
Bake Scene (wait)
Inspect My_Terrain_Scene
In Project, Terrain > Open • LightmapFar-0 and • LightmapNear-0
In Hierarchy Window, select Directional Light
In Inspector > Light > Intensity = 0
In Inspector: Light > Intensity = .5
Layer Pulldown Menu > Edit Layers
Rename Layer 8 = Terrain_Light_Culling_Layer
In Hierarchy Window, select Terrain
In Inspector Window > Terrain Pulldown Menu = Terrain_Light_Culling_Layer
In Hierarchy Window, select Directional Light
In Inspector Window, select Culling Mask Pulldown Menu = un√ Terrain_Light_Culling_Layer
Menubar > File > Save Scene As = My_Terrain_Scene