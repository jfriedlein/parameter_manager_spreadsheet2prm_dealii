# parameter_manager_spreadsheet2prm_dealii
Scripts to manage your parameters from deal.II in spreadsheets and export them by a single click to an auto-generated deal.II compatible prm-Parameters file

## What it does
Usually, parameters are managed in a "Parameters.prm" file based on the GeneralParameters class. So, if you want to change a parameter, you go into the prm file, opened with text editor and change the desired parameter. This works great, is super fast and independent of any operating system.

However, we you use parameter sets, so e.g. you test your models using a simple numerical example and then challenge it with a more demanding one, then you have to change lots of parameters. The straightforward approach would be to create two prm files and interchange the names to switch between the parameter sets. In a development environment, however, parameters might be added or disappear at any time, so in essence you have to keep up with two or more file and update them accordingly, which based on experience does work as long as a perpetuum mobile (in a paper dreamcastle forever, in reality it fails at first contact with the enemy).

That's what this script is for. You organise all your parameters in a spreadsheet and export the parameters and their values by single click to your prm file.

## Requirements
* LibreOffice Calc (currently supported, should be easily extendable to Excel, etc. transferring the macro)
* Python3 (not tested with Python2)

## Setup
The file `parameter_manager.xlsx` contains an example of a parameter set.
* To start, you have to download the spreadsheet, macro and the python script all into one folder (later the `maindir`).
* Open the Python script and change the output path `prm_output_dir` to the location where the final prm-file shall be placed.  
* Open the spreadsheet in LibreOffice Calc (currently the macro is only supported in LibreOffice Calc) and take a look around.
* Create an icon for the macro (refer to the website xyz)
* ...

@todo upload the macro somehow (or link it inside the spreadsheet)
