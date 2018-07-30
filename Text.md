ImageJ Training 2 180730 by Ryosuke TAJIMA  
==============  
  
# 1. Introduction  
- Macro is a simple program for automating some process in ImageJ  
- And plugin is also the other program for automating but I don't itroduce it today  
- Writing macro is much easier than writing plugin  

# 2. Using macro  
1. Open Image  
1. Select macro file: Plugins > Macros > Install...  
1. Run macro: Plugins > Macros > "CoverageOne"  
  
# 3. How to make your simple macro  
## 3-1. Recording your measurement  
1. Open Image  
1. Start recording: Plugins > Macros > Record...  
1. Record yout measurement  
    1. Split RGB: Image > Color > Split channels  
    1. Use image calculator: Process > Image calculator  
        1. Green (Substruct) Blue  
        1. Green (Substruct) Red  
        1. Green-Blue (Add) Green-Red  
    1. Theresholding: Image > Adjust > Threshold  
    1. Sometimes use invert: Edit > Invert  
    1. Analyze Particle: Analyze > Analyze Particle  
    (For coverage, use summarize)  
  
## 3-2. Test your record  
1. Select "Recorder" Window  
1. Click "Create": (Open "Macro.ijm.ijm (Running)" Window)  
1. Remove "//" from "//run("Threshold...")" (maybe at row 6)  
1. Open original image  
1. Click "Run"  

## 3-3. Modify  and your record  
1. Copy your record to txt file  
1. Control the name of images.  
    "selectImage" and "rename" are usuful.  
1. Save your modified macro  
1. Use your macro  
    1. Open Image  
    1. Select macro file: Plugins > Macros > Install...  
    1. Run macro: Plugins > Macros > "----"  

# 4. Developing your macro  
- You can modify and develop your macro if you get some more knowledge  
- e.g.  
    - function: Using "fuction", you can reuse for some situation in your macro.
    - for: Using "for" loop, you can open and analyse many image.  
