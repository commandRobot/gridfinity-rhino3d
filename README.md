# Gridfinity for Rhino3d

Overview:

This repository uses the GHops component within Grasshopper in Rhino3D to generate Gridfinity (https://gridfinity.xyz/ developed by Zack Freedman) modules automatically by controlling some key parameters such as count in X, Y, total height, divider height & height of bottom surface. 

By using the hops component, we are able to simplify the Grasshopper file into one only exposing the key parameters.
There will be a brief run through of the use of hosp below. 
For more information on how to use hops, go to https://developer.rhino3d.com/guides/compute/hops-component/. 

What is in this repository
1. readMe
2. gridfinity.ghx (source GHX file with GH definitions to be referenced when using hops)
3. gridfinity_HopsDefault.gh (template GH file to get started with using Gridfinity for Rhino3D in hops)

![gridfinity_hopsdefault](https://user-images.githubusercontent.com/12972773/223304858-33d589df-e880-4042-8c73-37ce384867cd.jpg)


# Gridfinity for Rhino3D Run Through

1. Open Rhino3D

2. Install Hops: First, you need to install the Hops plugin for Grasshopper. You can download the plugin from the food4Rhino website (https://www.food4rhino.com/en/app/hops) or install it using the Rhino Package Manager (search PackageManager in command line in Rhino3D).

3. Open Grasshopper: Open Grasshopper by typing "grasshopper" in the command line in Rhino3D.

4. Add a Hops component: To use Hops, you need to add a Hops component to your Grasshopper definition. You can do this by going to Params --> Util --> Hops. The easier way is to double-click or press the spacebar on the Grasshopper canvas & search for "Hops"

5. Pull gridfinity.ghx file into your local machine (alternatively, able to path the hops to https://github.com/commandRobot/gridfinity-rhino3d/raw/main/gridfinity.ghx , but that may not be working)

6. Connect your script to a Path: 
    There are 2 ways to connect your Hops component to the source Grasshopper Hops file 
    ![girdfinity](https://user-images.githubusercontent.com/12972773/223304207-c4f69cdc-f24e-4286-aa89-7346b739d3f2.jpg)
    
    1. Right-Click on the Hops component & select "Path". Then, select the gridfinity.ghx file from within your local machine
    2. Right-Click on the hops component & selct "Show Input: Path". Then open a Panel (right-click or space bar in GH canvas and search "Panel") and paste the permalink to the hops (https://github.com/commandRobot/gridfinity-rhino3d/raw/main/gridfinity.ghx)
The hop should now show the parameter inputs and output.

7. Customise: Customise your gridfinity by connecting various number sliders to the inputs. Ensure that your Hops visibility is turned on, so that the preview of the geometry appears in Rhino3D

8. Bake: Once you are happy with your gridfinity piece. Right click on hops and select "bake". This will bake your geometry into Rhino3D, where you will be able to export your file into your 3D printing slicer of choice for printing. (WIP: Bake button to directly bake ) 

Permalink to the file: https://github.com/commandRobot/gridfinity-rhino3d/raw/main/gridfinity.ghx

Screenshots for Reference
![image](https://user-images.githubusercontent.com/12972773/194511369-0ba00398-7775-4e81-bb4c-825875eab6b7.png)
![image](https://user-images.githubusercontent.com/12972773/194512291-a0d75fbc-f42f-40f6-b18b-3e87475e58a2.png)
