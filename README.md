# Installation
- Make sure that you have `python >= 3.6` installed. To see your python version, open your terminal and type: `python --version`
- navigate with your terminal to the cloned folder. E.g. `cd ~/housing-model/`
- choose one of the following possibilities to install the needed requirements
    - To install the needed librarys, either type: `pip3 install -r requirements.txt`
    - or, if you prefer anaconda, type: `conda install --file requirements.txt` in your terminal. 
    - Or, as third possibility, you can install the given librarys from requirements.txt directly from your packagemanager. With ubuntu, this should do the trick:`sudo apt install < requirements.txt`

# Inputs
The inputs can be finetuned and changed. You will find all inputs inside the input-folder.
- The `hyperparameter.xlsx` file contains: 
    - population developement variant (bev-variant)
    - scenario (choose either one single scenario, or comma-separated, or type `all`)
    - restauration_building_type bias (the yes-case is not yet implemented)
    - second_amb_restauration (the yes-case is not yet implemented)
    - output_folder (the folder relative to your housing-model path where you want the output to be saved)
- The `scenario_parameter.xlsx` file contains all defined scenarios. 
    - to create your own scenario simply add it directly below the last line in the same format with the same parameters as given. 
    - The divergence-cell can either contain one "global" value, which will be apllied on all years or four, which then will be applied once per decade.

# Data
The data that is used for this project can be found inside the data-folder.
- `12421-0001.xlsx`: Demographic developement of germany based on different population models [^1]
- `distribution_buildings.xlsx`: Distribution of demolition and restauration rate over building types
- `share_buildings_2019.xlsx`: Tabula-ID and calculated living space in million square meteres for 2019.  Weighting of the building typology in 2019 based on a weighted building
typology from 2011 [^2] and supplemented by energetic modernisation [^3] and new buildings and demolition
- `TABULA-Analyses_DE-Typology_ResultData.xlsx`: Main data ressource for calculating the model outputs. Building typology data from IWU (Institut Wohnen und Umwelt)[^4]








[^1]: [German Demographic Developement](https://www-genesis.destatis.de/genesis/online?operation=table&code=12421-0001&bypass=true&levelindex=0&levelid=1643115777925#abreadcrumb)
[^2]: [Weighted building typologiy from 2011](https://www.iwu.de/fileadmin/user_upload/dateien/energie/klima_altbau/Fl%C3%A4chen_Geb%C3%A4udetypologie_Okt_2013.pdf)
[^3]:[Energetic Modernisation](https://www.iwu.de/fileadmin/publikationen/gebaeudebestand/2018_IWU_CischinskyEtDiefenbach_Datenerhebung-Wohngeb%C3%A4udebestand-2016.pdf)
[^4]: [Tabula data table](https://www.iwu.de/fileadmin/tools/tabula/TABULA-Analyses_DE-Typology_DataTables.zip)