# Lesson Plan

Open terminal

Open GitHub in browser

##Set Up Project 1 Directory
* df
* cd PATH TO YOUR HD
* copy HTTPS clone URL
* git clone HTTPS URL
* cd into repository
* git init
* ls
* vi Readme.md
* i statement about this is your projects folder for VM364
* esc
* :wq
* mkdir Project 1
* ls
* cd Project 1
* touch Project1.md
* ls
* vi Project1.md
* i statement about this project
* esc
* :wq
* cd to root directory folder
* git status
* git add
* git commit
* git push

##Set up Unity in Project 1 Directory
* Open Unity
* Create new Project -> set in project 1 directory of your HD
* Menu Bar -> Unity -> Preferences -> Set external tools to MonoDevelop and Photoshop
* Create folders in project window (these can also be created in the directory)
	* _Scenes
	* _Materials
	* _Textures
	* _Prefabs
	* _Scripts
	* _Maya (Create this one in the directory)


## Set up Maya in Project 1 Directory
* Open Maya
* File -> Project -> New
* title Maya project
* Set location inside of Project 1 -> Unity Folder -> Assets Folder -> Maya Folder
* Use Defaults for folder names


## Push to git hub
* Check directories in Finder
* Check in Unity
* Go to Terminal
	* cd to project 1 directory if not in it
	* git status
	* git add
	* git commit
	* git push
* Look at your GitHub account

## Fork class folder
* Follow tutorial [Here](https://help.github.com/articles/fork-a-repo/)	

## Unity Interface Assetts

Create a New Project

Menu Bar > File > New Project

Set = Desktop/Lesson_One/Unity = My_Interface-Assets

√ Character Control.unityPackage

Create Project

Menu Bar > File > Save Scene As New Folder = Scene_01

In the Project Window > Create = Folder or Menu Bar – Assets > Create = Folder

Rename = Custom_Assets (Keep all custom assets that you create in a Custom_Assets folder so that they do not get mixed in with Standard Assets, this will make them portable and easy to use in subsequent projects)

In Inspector Window, select the Main Camera game object

Components

Transform Property Component: Position, Rotation and Scale

Camera Component:

GUI Layer Component:

Flair Layer Component:

Audio Listener: (only one per scene)

Game Objects

Menu Bar – GameObect > Create Other > Cube

Show Grid (landscape icon button, forth from left in Scene Window)

Rename = Door

Position X = 0

Position Y = 1.5

Position Z = -8

Scale X = 1.5

Scale Y = 3

Scale Z = .1

In Scene Window, select Door

f Key (frame selected)

Use your Cursor Arrows to navigate the scene

Use the Opt (Alt on Windows)+Left Mouse to tumble (just like Maya)

Use the Opt (Alt on Windows)+Middle Mouse to track (just like Maya)

Use the Opt (Alt on Windows)+Right Mouse or Scroll Wheel to dolly (just like Maya)

Select, Track, Tumble and Dolly Navigation Buttons (above left side of Scene Window)

Gizmo Navigation (upper left in Scene Window (like Maya but uses orthographic projection in Front, and Side)

Return to Perspective View

Transform Manipulators

X = Red Arrow

Y = Green Arrow

Z = Blue Arrow

w Key = Move game object (like Maya)

e Key = Rotate game object (like Maya)

r Key = Scale game object (like Maya)

Import Asset

Menu Bar > Asset > Import New Asset =
Lesson_01/Resources/Door_Color.jpg

Drag Crate_Color.jpg to Custom_Assets folder in Project Window

Assets > Create > Material

Rename = Door_Material

Drag Door_Material to Custom_Assets folder in Project Window

Select Door_Material

Drag Door_Color.jpg to Main Color attribute in Inspector Window

Select Door

Drag Door_Material to Inspector Window to add the component

Add Light

Game Object > Create > Directional Light

Position X = 0

Position Y = 2

Position Z = 0

Rotation X = 60

Rotation Y = 25

Rotation Z = 0

Asset > Import New Asset = Resources/Door_Bump.jpg

(a bumpmap creates the illusion od a bumpy surface by manipulating surface normals)

Drag Door_Bump.jpg to Custom_Assets folder in Project Window

Select Door_Material

In Inspector Window > Shader pull-down menu = Bumped Diffuse

Drag Door_Bump.jpg to Normalmap attribute in Inspector Window

“This texture is marked as a normal map” Fix Now

In Project Window, select Door_Bump

In Inspector Window, √ Generate from greyscale

Apply

In Inspector Window > Bumpiness = 0.025

Apply

Tumble to backside of door (normal map does not respond to ambient light)

Pivot/Center (pivot set in modeling application)

Set to Pivot

You can use a group node to offset pivots points in Unity

GameObject > Create > Empty

Rename = Henge

Position X = 0.75

Position Y = 0

Position Z = -8

In Hierarchy Window, drag Door to Henge

Select Henge

Set to Center

Rotate Y

Undo

Set to Pivot

Rotate Y

Undo

Menu Bar > File > Save Scene As New Folder = Scene_02

Menu Bar > GameObject > Create Other > Cube

Rename = Crate

Position X = 0

Position Y = .5

Position Z = 0

Menu Bar – Asset > Import New Asset =
Lesson_01/Resources/Crate_Color.jpg

Drag Crate_Color.jpg to Custom_Assets folder in Project Window

Assets > Create > Material

Rename = Crate_Material

Drag Crate_Material to Custom_Assets folder in Project Window

Select Crate_Material

Drag Crate_Color.jpg to Main Color attribute in Inspector Window

Select Crate

Drag Crate_Material to Inspector Window to add the component

Menu Bar > Asset > Import New Asset = Resources/Crate_Bump.jpg

Drag Crate_Bump.jpg to Custom_Assets folder in Project Window

Select Crate_Material

In Inspector Window > Shader pull-down menu = Bumped Diffuse

Drag Crate_Bump.jpg to Normalmap attribute in Inspector Window

Fix now

In Project Window, select Crate_Bump

In Inspector Window > √ Generate from greyscale and Bumpiness 0.025

Apply

Menu Bar > Save Scene As = Scene_03

Prefabs/Instantiation

Menu Bar > Assets > Create > Prefab

Rename = Crate_Prefab in Project Window

Drag to Custom_Assets folder

Drag Crate from Hierarchy Window to Crate_Prefab in Project Window (blue indicates connection)

Drag Crate_Prefab instance to Hierarchy (blue)

Position X = 0

Position Y = .5

Position Z = 4

Drag another Crate_Prefab instance to Hierarchy

Rename Falling_Crate_Prefab

Position X = 0

Position Y = 8

Position Z = 4

Rotation X = 40

Rotation Y = 0

Rotation Z = 40

Dolly and track as need to see all

in Project Window, select original Crate_Prefab

Scale XYZ = 3 (to scale all instances)

Scale XYZ = 1

Select the new instance in the Hierarchy Window

Scale XYZ = 2 (changes only the instance)

Scale XYZ = 1

Game Window

Menu Bar > GameObject > Create Other > Plane (note mesh collider Component this will keep the character from falling to oblivian)

Rename = Ground

Position X = 0

Position Y = 0

Position Z = 0

Scale X = 10

Scale Z = 10

Menu Bar > Asset > Import New Asset = Resources/Corrugated_Steel.jpg

Map the Corrugated_Steel texture to Ground by creating a new Ground_Material

In Hierarchy, select Ground > Ground_Material > Main Color > Tiling X and Y = 200

In Project Window, drag Standard Assets/Prefabs/First Person Controller to Hierarchy Window

In Hierarchy Window, select First Person Controller instance

Position X = 0

Position Y = 1

Position Z = -10

In Hierarchy Window, Delete Main Camera (only one Audio Listener)

Play Game

W-A-S-D (or cursor arrows) to navigate + Mouse to look

Try to navigate through door

Navigate off edge of Ground plane

Stop Game

Colliders

Select Door in Hierarchy

Right-Click > Remove Box Collider Component

Play Game

Try to navigate through Door

Stop Game

In Hierarchy Window, select Door

Menu Bar > Component > Physics > Box Collider

Rigid Body

In Hierarchy Window, select Falling_Crate_Prefab

Menu Bar – Component > Physics > Rigid Body

Add (will break connection with original prefab = white)

Rename Falling_Crate

Play Game

Stop Game

Menu Bar > Assets > Import Package = Physics Materials

In Hierarchy Window, select Falling_Crate

In Inspector Window > Box Collider Material = Bouncy

Play Game

Stop Game

In Inspector Window > Rigidbody > Drag = 1

Play Game

Stop Game

In Inspector Window > Box Collider Material = Wood

Play Game

Stop Game

Menu Bar > Save Scene As = Scene_04

Import Custom FBX File

In Mac OS Finder, drag Resources/Studio_Light folder to Project Window/Custom Assets

In Project Window, select Custom_Assets/Studio_Light/Studio_Light/Studio_Light (Mesh)

In (FBXImporter) > Scale Factor = 1 (the default will be 0.01 which make objects very tiny, a value of 1 will be a good match to regard grid values as equalling 1 meter in both Maya and Unity)

Apply

In Project Window, drag Studio_Light game object to Hierarchy

Position X = 4

Position Y = 0

Position Z = -1

In Hierarchy Window, open Studio_Light/Extension_01/Extension_02/Head/Lamp/Bulb

Menu Bar, GameObject > Create Other > Spotlight

Position X = 0

Position Y = 0

Position Z = 0

Intensity = 3

In Hierarchy, drag Spotlight to Bulb (child inherits transform values)

Position X = 0

Position Y = 0

Position Z = .5

Rotate XYZ = 0

Hierarchy: Head – Rotate Y

Hierarchy: Lamp – Rotate X

Hierarchy: Extension_01 – Position Y

Hierarchy: Extension_02 – Position Y

In Project Window, select Custom_Assets/Studio_Light/Matterials/studio_light-bulb_material

Dolly around to look at bulb

In Inspector Window > Shader > Self-Illumin > Diffuse

Play Game

Stop Game

Inspect Project Directory/Project Window

Custom Layout

Preset Layouts

Default Layout (factory settings)

Add/delete tabs

Menu Bar > Help > Unity Manual

Menu Bar > Help > Reference Manual

Menu Bar > Help > Scripting Manual

