# cyclica-beta
the second iteration of Cyclica web client, complete with an engine and design overhaul.

## what's new from alpha?
  we've changed from a stacking window manager to a tiling one- this was done as it is more tablet friendly, and allows for greater productivity. This feature is in alpha currently, so resizing isn't yet supported, though eventually we'll try and impliment dragging for tablets and keyboard shortcuts for a netbook form factors.
  
  ### What types of devices will cyclica beta support?
  * ###### Desk - Any device with a mouse and keyboard, assumes a `HIDPI` screen
  
  * ###### Laptop - Same as Desktop, touch targets may be larger to accomodate a touch screen.
  
  * ###### Slate - No Keyboard, only touch. Targets may be automatically enlarged, and gestures are emphasized. 
  
  * ###### Netbook - Slate device with keyboard and touch, but no mouse. Think along the lines of a Pixel C or iPad Pro. Shortcuts are present and touch targets may be auto-enlarged. Linux or windows apps may not work as well as android apps for obvious reasons. Screen may be smaller (<9in), though this certainly isn't a rule for netbook form factors. These devices would most likely be the best dev machines, striking a balance between being cheap and powerful.
  
  * ###### [MAYBE]Smartphone - Like `Slate`, but UI adapts to a single frame, with more frames shown in an overview mode. Linux/Windows may be used, though Android apps will be the main focus.  
  
  ### How do I install Cyclica Beta?
  ## *Running from Localhost*
  `mkdir cyclica-beta && cd cyclica-beta`
  `wget https://sourceforge.net/projects/turbovnc/files/2.2.2/turbovnc_2.2.2_amd64.deb/download && sudo dpkg -i download`
  `sudo /opt/TurboVNC/bin/vncserver`
  `wget https://github.com/novnc/noVNC/archive/v1.1.0.zip && sudo unzip noVNC-1.1.0.zip`
  `sudo apt install -f && sudo apt install websockify`
  `cd noVNC-1.1.0`
  `./utils/launch.sh --vnc localhost:5901`
   
   run the output of that inside of a browser of your choice. If VNC isn't working, make sure your desktop environment is supported.
   
  
  
  ## What's ready right now?
  Currently, Cyclica Beta is just an HTML Document. The backend code still needs to be written. 
