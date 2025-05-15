#  Reprodicible Research Archive Master Thesis
By: Jasmijn Bazen  
Date of creation: 12/05/2025  

Purpose: A fully resproducible research archive containing all relevant information to 
reproduce the results in my master thesis. With no need to change code.  

The Study: The aim of this research was to find out the effect of Motivation on Ability Estimates. This was done through a multi-group SEM model. First, both the TIMSS and PISA datasets were cleaned. Then, the data was split into two groups (50/50) to make a train and a test set. Afterwards, a multi-group SEM model was fitted to the train data. The best fitting model based on certain fit statistics and other indicators (see the report for a full explanation) was chosen. Next, the best fitting multi-group SEM model was fitted to the Test data. This fit was evaluated.  
The Data: Both datasets are anonymous open access data from Large-Scale Assessment Studies on students: TIMSS (https://timss2019.org/international-database/) and PISA (https://www.oecd.org/en/data/datasets/pisa-2018-database.html)  
  

## Folder structure  
ResearchArchiveMasterThesis  
├── 1.Pre-Processing  
│   ├── IntermediateData  
│   │   ├── PISAdata.RData  
│   │   ├── TIMSSdata.RData  
│   │   └── TIMSSMeantime.RData  
│   ├── RawData  
│   │   ├── pisa18_m.RDS  
│   │   └── TIMSS2019.Rdata  
│   ├── Scripts  
│   │   └── DataCleaning.Rmd  
│   └── README.md  
├── 1.Post-Processing  
│   ├── Output  
│   │   ├── Effort_histogram.png  
│   │   ├── fast_responses_histogram.png  
│   │   ├── FastStudents_barplot.png  
│   │   ├── gender_barplot.png  
│   │   ├── mean_response_time_histogram.png  
│   │   ├── nativeness_barplot.png  
│   │   ├── PV1_histogram.png  
│   │   ├── pv1_response_time_heatmaps_grid.png  
│   │   ├── PV2_histogram.png  
│   │   ├── PV3_histogram.png  
│   │   ├── PV4_histogram.png  
│   │   ├── PV5_histogram.png  
│   │   ├── response_time_histogram.png  
│   │   ├── slow_responses_histogram.png  
│   │   ├── SlowStudents_barplot.png  
│   │   └── unanswered_questions_histogram.png  
│   ├── Scripts  
│   │   └── DescriptiveStatistics.Rmd  
│   ├── SEMModelGraph  
│   │   ├── SEMModelBase.drawio  
│   │   ├── SEMModelBase.png  
│   │   ├── SEMModelPISANL.drawio  
│   │   ├── SEMModelPISANL.png  
│   │   ├── SEMModelPISAOthers.drawio  
│   │   ├── SEMModelPISAOthers.png  
│   │   ├── SEMModelTIMSSNL.drawio  
│   │   ├── SEMModelTIMSSNL.png  
│   │   ├── SEMModelTIMSSOthers.drawio  
│   │   └── SEMModelTIMSSOthers.png  
│   └── README.md  
├── Data  
│   └── TestTrainData.RData  
├── RequirementsAndEthics  
│   ├── EthicsStatement.md  
│   └── Requirements.md  
├── Results  
│   ├── TestModelSummary.txt  
│   └── TrainModelSummary.txt  
├── Scripts  
│   └── DataModelling.Rmd  
├── LICENSE.md  
├── README.md  
└── ResearchArchiveMasterThesis.Rproj  


All code (`DataCleaning.Rmd`, `DescriptiveStatistics.Rmd`, `DataModelling.Rmd`), `README.md` files, and DRAWIO files in the `\1.Post-Processing\SEMModelGraph` folder are human generated. 
The data in the `\1.Pre-Processing\IntermediateData` folder; the output in the `\1.Post-Processing\Output folder`; and the TXT files in the `\Results` folder are project-generated. 

## How to use:
Open `ResearchArchiveMasterThesis.Rproj` in RStudio.  
If you only want to run the analyses yourself, subsequently run the `DataModelling.Rmd` file from the `Scripts` folder. This will create the two TXT files in the `\Results` folder.  
If you also want to run the data cleaning, you may run the `DataCleaning.Rmd` file, from the `\1.Pre-Processing\Scripts` folder. This script will take data from the `\1.Pre-Processing\RawData` folder, save intermediate data in the `\1.Pre-Processing\IntermediateData` folder, and finally save the data to be used in the `DataModelling.Rmd` file to the `\Data` folder.  
If you want to run the script to create the graphs in the \2.Post-Processing\Output folder, you may run the DescriptiveStatistics.Rmd file in the 2.Post-Processing\Scripts folder.  
You may find an Ethics Statement and software requirements in the `\RequirementsAndEthics` folder. 

The PNG plots in the `\1.Post-Processing\SEMModelGraph` folder were created using the website 
https://app.diagrams.net/  
The files to adapt the plots end with `.drawio` in the same folder and can be opened using the website, or their desktop appplication. 

This research archive is available at https://github.com/MagicXIV/ResearchArchiveMasterThesis.git  
This site will be maintained for at least a month by the main researcher (contact details below). The archive is publically available.  

Please note: The file `TIMSSMeantime.RData` in the `\1.Pre-Processing\IntermediateData` is not available on the Github repository due to the file size being too large. However, this file can be created by running the `DataCleaning.Rmd` file from the `\1.Pre-Processing\Scripts` folder. The `TIMSSMeantime.RData` file is not needed to run either the `DataModelling.Rmd` file from the Scripts folder or the `DescriptiveStatistics.Rmd` file from the `\2.Post-Processing\Output` folder.  

## License 
  
MIT License  
  
Copyright (c) 2025 Jasmijn L. Bazen

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:  
  
The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.  
  
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.  
  

## Contact information  
Jasmijn L. Bazen  
Student number / Solis ID: 2319020  
j.l.bazen@students.uu.nl  
