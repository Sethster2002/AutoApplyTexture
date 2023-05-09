# AutoApplyTexture
Scripts for automatically applying textures to various software. The scripts require specific naming conventions for the textures, so be sure to go through the README thoroughly to ensure that the programs will work properly for your models.

UNREAL:
  This script will bring up an interactive window that will allow you to automatically apply textures to multiple materials on multiple objects at once. 
  
  To set up the Unreal Editor to be able to properly run the script, you will need to enable Unreal's python plug-in and set the directory the Editor will use to find the script. First, go to "Edit/Plugins" in Unreal. In the Plugins window search bar type in "Python" and click the checkbox next to the option titled "Python Editor Script Plugin" if it is not already activated. Then, go to "Edit/Project Settings". In the Project Setting window search bar type "Python". Under the Python dropdown menu, find Additional Paths, and select the circled "+" button. This will add an index to the Additional Paths. In the newly created index, click the "..." button and set the path to the folder that contains the "AutoApplyTextures_Unreal.py" file. It is reccomended that you put the script in the content folder in a new folder titled "Scripts" or "Python". Once this path is set, you will be prompted to restart Unreal to apply the new settings. If you do not get this prompt, manually restart to program after saving to ensure that it will properlly read the script.
  
  Your project is now set up to use Python scripts in the editor. Now, select the static meshes you wish to apply materials to in either the Outliner or the Content Browser. Once your have your selection, you can click on "Tools/Execute Python Script..." (you may need to scroll down to find it). Now navigate to the folder you put the "AutoApplyTexture_Unreal.py" script and select the file. This will open an interactive window.


  Before setting any values, ensure that in the list titled "Selected Objects:", you see all the static meshes you wish to automatically apply textures to. The program defaults to using the actors selected in the outliner, but you can change the selection set to the content browser by clicking "Switch Between Outliner/Content Selection"
  
  If you want to only apply textures to certain materials on the mesh, click the "Toggle Material Selection" button. This will display a list of all the materials attatched to the first static mesh selected. This function will only affect the first mesh selected shown in the "Selected Objects" list, so it is recommended that you only select the mesh you with to work with. In this list, you can select each material you wish to apply textures to. Then, procede with the rest of the map selection process as normal.
  
  If your texture path is NOT SET, select "Set Texture Path" and navigate to the folder your textures are in. This can be used if you have multiple iterations/versions of an object's texture, simply place the seperate version in a different folder. If multiple versions of the same texture are in the same directory, the software with select the one with the highest version number. In this case, if the files don't have a version number, then it will randomly select one of the files, so be sure to use version numbers or put different versions into seperate folders.

  Under the "Plug into Which Propert?" label, select which property/properties the map will plug into. If you have not set a map ID value yet, the defualt ID will be automatically set. Then, you can set whether the texture should be interpereted as an sRGB or Raw (linear color) file.

