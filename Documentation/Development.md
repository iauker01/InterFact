
# Technology Stack: 

  • Internet connected camera hardware - Sends image data periodically to interfact.camera@gmail.com
  
  • StatusChecker Python program - Processes image data for presance of trains
  
  • SQL Database - Stores the status of the intersection & archives for future predictive features
  
  • Firebase - Stores the latest state for each intersection for system access
  
  • Angular - Front end development
  
  • ArcGIS - Plugin to overlay status on map


# Replicating Development Enviornment: 

## Code:
1. Download [Anaconda](https://www.anaconda.com/download/success) with python version 3.12
2. Install Anaconda; the default values are fine.
3. Open Anaconda Prompt
4. In prompt:
   * `conda create --name interfact`
   *  type y to proceed
   * `conda activate interfact`
   * install packages as written on requirements.txt file using either conda install or pip install

## ArcGIS Plugin:
  
    1.) Download the plugin file
    
      a.) Extract the plugin to ArcGIS program files (C:\Program Files\ArcGIS\Plugins)
      
      b.) Restart ArcGIS
      
    2.) Enable plugin through ArcGIS
    
      a.) In ArcGIS, navigate to: Customize > Extensions OR Tools > Extensions
      
      b.) Check the box next to "Interfact" plugin to enabvle it



# File & Folder Structure: 

    INSERT IMAGE OF STARTING FILE FOLDERS HERE
    
    • This is the main folder of the Interfact System. Main runnable project files will be located in the Auxiliary Files folder, layout & design files are located in the Design folder, client meeting details are located in the Discovery folder, the Meeting Minutes folder contains team meeting dates and details, the Documentation folder contains the development and deployment files, and the Presentations folder contains files related to Interfact team presentations.
