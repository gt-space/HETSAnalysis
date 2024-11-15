# HETSAnalysis
GUI for HETS Data Analysis.

### Using Github
If you have never used Github, this is how to properly install this GUI and update it when new updates are pushed.
1. Open the terminal on your computer and navigate to the folder in which you want the GUI. Use ```ls``` to look inside your current folder and ```cd _folder_``` to move to a deeper one.
2. Run ```git clone https://github.com/gt-space/HETSAnalysis.git```. This will create a version of the GUI on your computer. You can now run StahlDataAnalysis.mlapp from the file explorer like a normal application.
3. When new updates are pushed, run ```git pull origin main``` from the HETSAnalysis file to receive the update. The number at the bottom of the GUI should match the number in the commit message in Github.

### Using the GUI
1. Before opening the GUI, put the desired data file into the same folder as the GUI.
2. Open the GUI. Type the name of the file, including the extension, into the 'data file' box. The GUI can use either .csv or .mat files.
3. Navigate to the 'Load Inputs' tab. Click the desired injector - subscale ablative is labelled as such because the desired MR is different from subscale heatsink. Ensure the dataset values are correct, change them if necessary, and press the 'Load' button to load them into the 'Main' tab.

    *If the dataset values are taking a long time to load, you can enter them manually in the 'Main' tab.
5. Navigate back to the 'Main' tab. Change the settings based on the to-be-analyzed dataset. In step 3, the values 'LOX Orifice CdA', 'LOX System CdA', 'Fuel Orifice CdA', and 'Fuel System CdA' were changed as well as the center data inputs, so do not worry about them.
6. Press 'Run' to analyze the dataset. The dataset will be analyzed when the box to the right of the 'Run' button reads 'Finished!'. This box will change back to 'Not running.' after 5 seconds, do not worry.
7. Navigate to the 'Plots' tab to generate plots from the analyzed dataset.

### Viewing and editing the code
If there seems to be a problem with the output data file or if you want to make changes to the analysis, you may need to view the code.
1. Open Matlab.
2. Navigate to the 'APPS' tab in the blue banner.
3. Click 'Design App' in the grey header.
4. Click 'Open...' and find the GUI in File Explorer.
5. You are now editing the GUI on your computer. Switch to 'Code View' to see the code.

### Errors
If the code is halted for a very long time, there may be an error. If there is, it will appear in the MATLAB terminal and in App Designer if it is open.
Note that the code takes a long time on Processing (3/4) and Running (4/12) due to the data parsing occuring in those sections. This is normal, especially with Spring '24 data where the datasets are substantially larger than the respective fire time.
