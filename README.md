# Instructions
## Abstract

Importance:  Phase I cancer studies, which guide dose selection for subsequent studies, are almost three times more prevalent than Phase III studies and have a median study duration well-over 2 years, comprising a major component of drug development time.  Objective: We seek to reduce the duration of Phase I studies in adult and pediatric cancer studies without violating risk-limits by better accommodating the accrual and evaluation process (“queue”).  Design: The processes modeled, the Phase I Queue (IQ), includes patient inter-arrival time, screening, and dose-limiting toxicity evaluation. For our proof-of-principle, the rules of the 3+3 and Rolling 6 Phase I designs were modified to improve patient flow through the queue without exceeding the maximum risk permitted in the parent design. The resulting designs, the IQ 3+3 and IQ Rolling 6, were compared to their parent design by simulation in twelve different scenarios.  Main Outcome and Measures: (1) Time from study open to determination of the Maximum Tolerated Dose (MTD); (2) Number of patients treated to determine the MTD; (3) Impact on the dose selected as the MTD. Results: Based on 800 simulations, for all 12 scenarios considered, the IQ 3+3 and the IQ Rolling 6 designs reduced the expected study duration compared to the parent design.  The expected IQ 3+3 reduction ranged from 1.6-10.4 months (3.7 months for the “standard” scenario), and the expected IQ Rolling 6 reduction ranged from 0.4 to 10.5 months (3.4 months for the standard scenario).  The increase in the average number of patients treated in the IQ 3+3 compared to the 3+3 ranged from 0.6 to 3.2. No increase in the number of patients was associated with the IQ Rolling 6 when compared to the Rolling 6 design. Effect on the probability of selecting a dose as the MTD was <3% for all doses, scenarios and both parent designs. Conclusions and Relevance: We demonstrate that IQ designs can reduce the average duration of Phase I studies as compared to their parent designs without changing the risk-limits or MTD selection operating characteristics.  These approaches have been successfully implemented in both hematology and solid tumor Phase I studies.  

## FlexSim Health Care

Before beginning to run simulations, make sure you have registered and logged onto FlexSimHC (https://flexsim.com/clinical-trials), and downloaded the FlexSimHC module. You should also see a serial number to activate the module. To activate, go to the Help menu -> Liscence Activation, and provide the Activation ID and click Activate. 

## Run the model

Download the model named "IQdesigns" and the xlsx decision grid data provided above. 

Open up the FlexSimHC software, on the left panel, click "Open Model", select the IQ designs model you just downloaded, this step might take a while. Now on the right panel, click thee Excel icon next to the "Experiment" button and select the excel file you just downloaded and wait for the file to be imported. After that, click the "Experiment" button. 

Click the "Experiment Run" tab and customize how many replications you want, the default is 800. Click "Run Experiment". 

Now you will hear your pc fan running like it's going to explode. 

Once the experiment is complete, you have the option to export results for further analysis, just select the "DataCollector1" table under Data History Tables and click export data. 










