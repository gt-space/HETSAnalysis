# HETSAnalysis
GUI for HETS Data Analysis.

### Using Github
If you have never used Github, this is how to properly install this GUI and update it when new updates are pushed.
1. Open the terminal on your computer and navigate to the folder in which you want the GUI. Use 'ls' to look inside your current folder and 'cd _folder_' to move to a deeper one.
2. Run 'git clone https://github.com/gt-space/HETSAnalysis.git'. This will create a version of the GUI on your computer. You can run it from the file explorer like a normal application.
3. When new updates are pushed, run 'git pull origin main' to receive the update. The number at the bottom of the GUI should match the number in the commit message in Github.

### Using the GUI
1. Before opening the GUI, put the desired data file into the same folder as the GUI.
2. Open the GUI. Type the name of the file, including the extension, into the 'data file' box. The GUI can use either .csv or .mat files; if any problems arise with a .mat file, convert it to a .csv file and file a complaint with Jackson Stahl.
3. Navigate to the 'Load Inputs' tab. Click the desired injector - subscale ablative is labelled as such because the desired MR is different from subscale heatsink. Ensure the dataset values are correct, change them if necessary, and press the 'Load' button to load them into the 'Main' tab.
4. Navigate back to the 'Main' tab. Change the settings based on the to-be-analyzed dataset. In step 3, the values 'LOX Orifice CdA', 'LOX System CdA', 'Fuel Orifice CdA', and 'Fuel System CdA' were changed, so do not worry about them.
5. Press 'Run' to analyze the dataset. The dataset will be analyzed when the box to the right of the 'Run' button reads 'Finished!'. This box will change back to 'Not running.' after 5 seconds, do not worry.
6. Navigate to the 'Plots' tab to generate plots from the analyzed dataset.

### Viewing and editing the code
If there seems to be a problem with the output data file, or if a sensor was swapped with another and the plots need to reflect that, you may need to view the code.
1. Open Matlab.
2. Navigate to the 'APPS' tab in the blue banner.
3. Click 'Design App' in the grey header.
4. Click 'Open...' and find the GUI.
5. You are now editing the GUI on your computer. Switch to 'Code View' to see the code.
