# AutoApplyTexture
Scripts for automatically applying textures to various software. The scripts require specific naming conventions for the textures, so be sure to go through the README thoroughly to ensure that the programs will work properly for your models.

UNREAL:
  Before setting any values, ensure that in the list titled "Selected Objects:", you see all the static meshes you wish to automatically apply textures to. The 
  program defaults to using the actors selected in the outliner, but you can change the selection set to the content browser by clicking "Switch Between   
  Outliner/Content Selection"
  
  If your texture path is NOT SET, select "Set Texture Path" and navigate to the folder your textures are in. This can be used if you have multiple 
  iterations/versions of an object's texture, simply place the seperate version in a different folder. If multiple versions of the same texture are in the same 
  directory, the software with select the one with the highest version number. In this case, if the files don't have a version number, then it will randomly select 

  Under the "Plug into Which Propert?" label, select which property/properties the map will plug into. If you have not set a map ID value yet, the defualt ID will be
  automatically set. Then, you can set whether the texture should be interpereted as an sRGB or Raw (linear color) file.

