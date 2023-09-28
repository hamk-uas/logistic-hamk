# logistic-hamk
Python Streamlit App to get user input data for logistic simulation (logistics_sim)
Whith this app you can enter your input data for processing in logistic simulation (logistics_sim). 

First, you need to choose in sidebar menu how you want to provide input data for places and depots,it can be:
1)Random Addresses Generator: enter the numbers and area (rectangle) to generate random addresses
2)Manually type the addresses and optionally names for the places
3)Addresses from your CSV: upload your CSV file with location data and select the corresponding column (columns)
After saving all files to the Azure blob storage press start. It will activate virtual machine that will make all the calculations. After that you can see the result on the map and download result files to you computer. After you press start it takes from 5min to hours, depend how many addresses you have and how many days of simulation you need.
For sensitive information I used Keyvault, VM will be stopped automaticcally after all calculation will be made.
