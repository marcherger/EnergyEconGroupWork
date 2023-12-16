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
This file downloads the electricity load and the intermittent supply from the ENTSO-e transparency platform. These files are then stored in */EnergyEconGroupWork\DownloadDataForDK\CleanedData*.

### *B_DownloadFromEnergyDataService.ipynb* 
We are not using this file as we abstract from transmission. 

### *C_DownloadFromClimateOutlook.ipynb*
This file downloads the plant data from the Danish Climate Outlook and stores this data in */EnergyEconGroupWork\DownloadDataForDK\CleanedData*.

### *D_MakeModelData.ipynb*
This takess the pickle files stored in */EnergyEconGroupWork\DownloadDataForDK\CleanedData* as well as additional data to creat the excel files in the folder */EnergyEconGroupWork\DownloadDataForDK\ModelData*.

## Data Construction
### *0_Construct_Final_Dataset.ipynb*
This file can be found in */EnergyEconGroupWork/DownloadDataForDK/ModelData*. It creates the Excel sheets in */EnergyEconGroupWork/DownloadDataForDK/ModelData/Final_Dataset* using the files stored in */EnergyEconGroupWork\DownloadDataForDK\ModelData*. 

At the end of the jupyter notebook the files in */EnergyEconGroupWork/DownloadDataForDK/ModelData/Final_Dataset*, which are the seperate sheets of the data going into the model, are put together to one file called *mBasicPH_storage_Data.xlsx* and is then stored in */EnergyEconGroupWork/Data*

## Model Analysis
The analysis of the model takes place within the *Analysis_mBasicPH_storage.ipynb* file. It utilizes the *.py* files from the folder */EnergyEconGroupWork/py*. Those *.py* files originate from */EnergyEcon/EnergyEconomicsE2023/py*. We made only minor adjustments to the *mBasicPH_storage.py* file. Namely, adjusting the names of the generaors to make sure they align with our dataset.