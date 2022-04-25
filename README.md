The Hyperparameter file contains: population developement and the scenarios can be choosed here. 
The scenario_parameter file contains the scenarios, but just those called in the Hyperparameter file will be calculated. 
The divergence-cell can either contain one "global" value, which will be apllied on all years or four, which than will be applied on each zwischen-value.
Bevölkerung durch 1000 teilen 
Formeln für die Berechnung der newe_building und demolition rate von der min rate beschreiben

To install the needed librarys type:
pip3 install -r requirements.txt

if you prefer anaconda, try:
conda install --file requirements.txt

you can also install the given librarys from requirements.txt directly from your packagemanager

cat requirements.txt | xargs apt install -y