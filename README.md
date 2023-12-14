# EnergyEconGroupWork
Git Repository for the exam project of Group 9. 
| Group Members              |
|----------------------------|
| Name                       | Email                       |
|----------------------------|-----------------------------|
| Marc Andreas Herger        | kvt932@alumni.ku.dk         |
| Paul Gabriel Martin Meißner| wls881@alumni.ku.dk         |
| Carolus Siikanen           | nsf767@alumni.ku.dk         |

The following document gives a brief overview how we structured the repository and how we constructed our dataset.

## Data Download
The files for the data download can be found in the folder */EnergyEconGroupWork/DownloadDataForDK*
They originate from */EnergyEconomicsE2023/DownloadDataForDK*

### *A_DownloadFromENTSOe.ipynb*
This file downloads the XXX. 

### *B_DownloadFromEnergyDataService.ipynb* 
We are not using this file as we abstract from transmission. 

### *C_DownloadFromClimateOutlook.ipynb*
This file downloads the XXX. 

### *D_MakeModelData.ipynb*
This file creates the pickle files in the folder */EnergyEconGroupWork/DownloadDataForDK/CleanedData*

## Data Construction
### *0_Construct_Final_Dataset.ipynb*
This file can be found in */EnergyEconGroupWork/DownloadDataForDK/ModelData*. It creates the Excel sheets in */EnergyEconGroupWork/DownloadDataForDK/ModelData/Final_Dataset* which are then put together to create the final dataset. This final Excel file called *mBasicPH_storage_Data.xlsx* is then stored in */EnergyEconGroupWork/Data*

## Model Analysis
The analysis of the model takes place within the *Analysis_mBasicPH_storage.ipynb* file. It utilizes the *.py* files from the folder */EnergyEconGroupWork/py*. Those *.py* files originate from */Users/paul/EnergyEcon/EnergyEconomicsE2023/py*. We made only minor adjustments to the *mBasicPH_storage.py* file. Namely, adjusting the names of the generaors to make sure they align with our dataset.