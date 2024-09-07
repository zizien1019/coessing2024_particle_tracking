Last updated Aug 2024, Zih-En Tseng

This notebook utilizes the model output of ECCO (Estimating the Circulation and Climate of the Ocean), version 4 release 4,
alongside with the Parcels (Probably A Really Computationally Efficient Lagrangian Simulator),
to perform 2-D and 3-D particle tracking simulation in the global ocean.

For more information about ECCO, please visit:
    https://www.ecco-group.org/home.htm

For more information about Parcels, please visit:
    https://oceanparcels.org/


Install and run guide:
ECCO-GROUP/ECCO-v4-Python-Tutorial/master/ECCO-ACCESS/ecco_download.py

1. Environment setup
   It is recommended to run the notebook with a clean conda environment to avoid messing up with other part of your computer.
   One can find miniconda distribution online:
   
     https://docs.anaconda.com/miniconda/
   
   Once you installed miniconda on your computer, create a fresh environment for the packages.
   This can be achieved with comments:
   (replace ENVNAME with any name you want for your environment)
   
         conda create -n ENVNAME

   Once you have the environment, activate it and install all packages required.
   
         conda activate ENVNAME
   
         conda config --add channels conda-forge
   
         conda install --channel=conda-forget numpy xarray xgcm xmitgcm pyresample trajan parcels

3. Accessing ECCOv4r4 model output data
   One must have an active NASA Earth data account to access the ECCO data online.
   
     https://www.earthdata.nasa.gov/

   With a NASA Earthdata account, you will have access to even more incredible data from the most avant-garde projects happening on this planet!
   For example, CYGNSS satellite project, in which I myself is also included and working on the assess the distribution of plastic waste in ocean.
   
   One is also referred to the github repo of the ECCO team for more tools and examples on how to access and process the data:
   
   https://github.com/ECCO-GROUP/ECCO-v4-Python-Tutorial/
   
   In the notebook, I utilized the download routine to help browse and organize the downloaded data with function ecco_download.py,
   this function can be found here:
   
   https://github.com/ECCO-GROUP/ECCO-v4-Python-Tutorial/tree/master/ECCO-ACCESS/ecco_download.py

   It is necessary to link this function within your working environment's scope.

5. Have fun with the code! Make your hands dirty!

6. It must be noted that the current state of this notebook is not robust enough to account for true distance traveled by ocean currents.









