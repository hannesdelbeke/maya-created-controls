A control creator for Maya (written in Mel)  
Tested in Maya 2026. Most of this was created in Maya 2022.  

A maya module based on the original script written by stac9350 
> Stanislav Slavyanov     
> telegram - @stac9350  
> mail - stac9350@gmail.com

- [watch](https://youtu.be/vVcceGPmFYk?si=5axL7MENpLXDv39Q) a demo on youtube 
- download the original script on artstation [here](https://www.artstation.com/marketplace/p/DBXx0/maya-script-created-controls)  

 
![image](https://github.com/user-attachments/assets/082ca02a-e1a5-454c-b615-537646f9bd4a)

## updates in this repo
- packages the control creator in a Maya module for easy distribution, without needing to edit the code
- fix some bugs
  - Y & Z procs are just copy pasted from X, but not renamed
  - there was some clipping in the bottom of the UI
  - When I try run it from python or using `source` in [[Maya MEL|mel]], i notice the non global procs don't work. I convert them to global.
  - When I add the file in the maya script path, and run it from mel with the script name, it doesn't work because there's a `.` in the name. convert this to `_` fixes that.
- wrapped this script in a python plugin so it can be enabled/disabled

## Plugget
_To be used as a demo repo to test Maya module installations with [plugget](https://github.com/plugget/plugget)_
