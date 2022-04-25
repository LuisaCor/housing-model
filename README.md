# Installation
- Make sure that you have `python >= 3.6` installed. To see your python version, open your terminal and type: `python --version`
- navigate with your terminal to the cloned folder. E.g. `cd ~/housing-model/`
- choose one of the following possibilities to install the needed requirements
1. To install the needed librarys, either type: `pip3 install -r requirements.txt`
2. or, if you prefer anaconda, type: `conda install --file requirements.txt` in your terminal. 
3. you can also install the given librarys from requirements.txt directly from your packagemanager. With ubuntu, this should do the trick:`sudo apt install < requirements.txt`

# Inputs
The Hyperparameter file contains: population developement and the scenarios can be choosed here. 
The scenario_parameter file contains the scenarios, but just those called in the Hyperparameter file will be calculated. 
The divergence-cell can either contain one "global" value, which will be apllied on all years or four, which than will be applied on each zwischen-value.
Bevölkerung durch 1000 teilen 
Formeln für die Berechnung der newe_building und demolition rate von der min rate beschreiben

