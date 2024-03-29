# Script to Access Census APIs
The script in this directory is used to grab census data from the group of census APIs. It currently work with the Decennial census and the ACS. It will work with other APIs with minimal changes.

To prepare to run, simply run the command: 
````
pip install --upgrade -r requirements.txt
````
There are several text files that are used by this script:
- keyfile.json (ignored by git), where your should store your api key
- inputs.json, where you should input the parameters that you're looking for
- CensusCodes.csv, where you should have a list of the codes of census tables that you're interested in.

There's a jupyter notebook file as well, which shows how to explore and filter through census codes from the api, and generate the CensusCodes.csv file. (It's helpful to filter through the codes in this way, as copying and pasting many census codes is a hassle). The format of this csv matters, so use the jupyter notebook file as a guide to generate your own.

## Formatting Census Data

This script will format the data by replacing census codes with what they represent, if the CensusCodes.csv file is formatted correctly. If you need a slightly different format, you'll have to edit the script a bit.
