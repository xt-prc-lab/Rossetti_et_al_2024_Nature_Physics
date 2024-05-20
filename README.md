# INTRO
This repository contains the MATLAB scripts used for data processing and analysis in the publication “Optogenetic generation of leader cells reveals a force-velocity relation for collective cell migration” – accepted in Nature Physics (bibliographical information will be added when available).

# DISCLAIMER
These scripts were written for personal use. They consist of very basic, poorly planned and inelegant coding. There are many repetitions, dead ends, and unused sections. They are not appropriately commented, structured or documented for external users. If you are interested in using all or some pieces of these scripts, please contact the author (see below) and you will receive detailed personalized explanations.
These scripts are made freely available so that interested readers of the paper can access, and verify, how data was processed and analysed.

# DESCRIPTION
First, Traction Force computations were performed using previously published scripts, as cited in the paper. These scripts are not included here and are available from Xavier Trepat ([xtrepat\@ibecbarcelona.eu](mailto:xtrepat@ibecbarcelona.eu?subject=Traction%20Force%20Microscopy%20Code)) upon request. The outputs (.dat files, and .mat files) of the Traction Force code are required to run the scripts in this repository.

The pipeline is applied as follows for each individual experiment (for singlets, doublets etc. separately): first the script CoL_561analyzer.m is run, followed by CoL_cellgroup_tractions_analyzer.m. These scripts will save variables in a folder that acts as a database (Cell_Singlet_Analysis_Database etc.). Finally, when all experiments are analyzed, the script CoL_MAIN_Analysis_Code.m is run (individually for each length of the cell trains). This script performs accesses the database folders and performs the final analyses, also generating the plots for the paper.

# CONTACT
For all script-related matters contact Leone Rossetti ([lrossetti\@ibecbarcelona.eu](mailto:lrossetti@ibecbarcelona.eu?subject=Rossetti%20et%20al%202014%20Scripts), [l.rossetti@kcl.ac.uk](mailto:l.rossetti@kcl.ac.uk?subject=Rossetti%20et%20al%202014%20Scripts))
