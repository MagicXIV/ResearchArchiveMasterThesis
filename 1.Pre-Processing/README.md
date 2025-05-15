# Pre-Processing Folder  
By: Jasmijn Bazen  
Date of creation: 15/05/2025  

Purpose: A folder which contains all files to transform the raw data in the RawData folder
to the data in the main Data folder to be used for the data modelling.  


## The folder structure  

1.Pre-Processing  
├── IntermediateData  
│   ├── PISAdata.RData  
│   ├── TIMSSdata.RData  
│   └── TIMSSMeantime.RData  
├── RawData  
│   ├── pisa18_m.RDS  
│   └── TIMSS2019.Rdata  
├── Scripts  
│   └── DataCleaning.Rmd  
└── README.md  

The code (DataCleaning.Rmd) and the README.md file are human-generated.
The data in the IntermediateData folder are project-generated. 

Please note: The file TIMSSMeantime.RData in the \1.Pre-Processing\IntermediateData is not available on the Github repository due to the file size being too large. However, this file can be created by running the DataCleaning.Rmd file from the \1.Pre-Processing\Scripts folder. The TIMSSMeantime.RData file is not needed to run either the DataModelling.Rmd file from the Scripts folder or the DescriptiveStatistics.Rmd file from the \2.Post-Processing\Output folder.  
