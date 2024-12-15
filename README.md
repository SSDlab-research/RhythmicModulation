# RhythmicModulation

To analyze kinematic data, …
- Run the standalone application run_KinematicModApp.sh, either in a MATLAB environment using the system command (see example below) or in the terminal (only requires a MATLAB Runtime installation without the need for a licensed copy of MATLAB)
- A new file named data_kinematic_modulation.txt will be generated, containing all kinematic features in the reference. 
- The specific instructions for running a standalone application can be found here: https://www.mathworks.com/help/compiler/create-standalone-app-from-matlab-function.html#CreateStandaloneApplicationFromMATLABFunctionExample-9. 

Example: 
- In MATLAB, navigate to the KinematicModAppstandaloneApplication directory and run the following code: system(['./KinematicModAppstandaloneApplication/run_KinematicModApp.sh ', matlabroot,' DIRECTORY'])
- Replace DIRECTORY with the specific directory name where the kinematic data are located. Some sample data are provided in the Test_kinematic folder. This folder should contain the following: 
1) Kinematic data (*.txt file with 16 columns corresponding to ULz, ULy, LLz, LLy, T1z, T1y, T2z, T2y, T3z, T3y, T4z, T4y, J1z, J1y, J2z, J2y, where z is superior-inferior and y is anterior-posterior)
2) Time stamps (*-tags.txt file with three columns corresponding to the time stamps, data source [e.g., “Audio”], and transcription, respectively.)


To analyze acoustic data, …
- Run the standalone application run_AcousticModApp.sh, either in a MATLAB environment using the system command (see example below) or in the terminal. 
- A new file named data_acoustic_modulation.txt will be generated, containing all acoustic features in the reference. 

Example: 
- In MATLAB, navigate to the AcousticModAppstandaloneApplication directory and run the following code: system(['./AcousticModAppstandaloneApplication/run_AcousticModApp.sh ', matlabroot,' DIRECTORY'])
- Replace DIRECTORY with the specific directory name where the acoustic data are located. Some sample data are provided in the Test_acoustic folder. This folder should contain the following: 
1) Acoustic data (*.WAV files)
2) Time stamps (*-tags.txt files, in the same format as above)

