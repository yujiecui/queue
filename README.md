# Instructions

## FlexSimHC Download

Before beginning to run simulations, make sure you have registered and logged onto [FlexSimHC](https://flexsim.com/clinical-trials), and downloaded the FlexSimHC module. You should also see a serial number to activate the module. To activate, go to the Help menu -> Liscence Activation, and provide the Activation ID and click Activate. 

Watch the intro video here, or go to [FlexSimHC](https://flexsim.com/clinical-trials) website for general questions about the software.

[![IMAGE ALT TEXT](http://img.youtube.com/vi/oAgYD6WnWis/0.jpg)](https://www.youtube.com/watch?v=oAgYD6WnWis "Video Title")


## Run the model

See the instructions.pdf above for more details on how to run a simulation model for the first time. 

To run the IQ designs, download the model named "IQdesigns" and the xlsx decision grid data provided above. 

Open up the FlexSimHC software, on the left panel, click "Open Model" and select the IQ designs model (the .fsm file) you just downloaded. This step might take a while.

Now on the right panel, click the Excel icon next to the "Experiment" button and select the excel file you just downloaded and wait for the file to be imported. After that, click the "Experiment" button. 

Click the "Experiment Run" tab and customize how many replications you want, the default is 800. Click "Run Experiment". 

Now you will hear your pc fan running like it's going to explode. 

Once the experiment is complete, you have the option to export results for further analysis, just select the "DataCollector1" table under Data History Tables and click export data. 

# Analysis using R


```R
library(tidyverse)
library(janitor)

# calculate months from days
months<-function (days) {
  12*days/365.25
  }
  
  
data <- read.csv("DataCollector1.csv")  # this is flexsim output


```

Summary of study duration, number of patients started treatment, etc. 
```R
# Summary - Number started treatment
data %>% group_by(Scenario) %>% 
summarise(mean = mean(NumStartTreatment), median= median(NumStartTreatment), range = range(NumStartTreatment))  # N started treatmetn at each design


# Summary - study length in months
data %>% group_by(Scenario) %>% 
summarise(mean = mean(months(StudyLength)), median = median(months(StudyLength)), range = range(months(StudyLength)))  # Study length in months.

# overdose rate

data %>% mutate(overdose_rate = NumDLTsAboveMTD/NumFullyEvaluated) %>% 
  group_by(Scenario) %>% 
  summarise(mean = mean(overdose_rate))
  

```









