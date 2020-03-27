# Instructions

We seek to reduce the duration of Phase I studies in adult and pediatric cancer studies without violating risk-limits by better accommodating the accrual and evaluation process (“queue”). The processes modeled, the Phase I Queue (IQ), includes patient inter-arrival time, screening, and dose-limiting toxicity evaluation. For our proof-of-principle, the rules of the 3+3 and Rolling 6 Phase I designs were modified to improve patient flow through the queue without exceeding the maximum risk permitted in the parent design. The resulting designs, the IQ 3+3 and IQ Rolling 6, were compared to their parent design by simulation in twelve different scenarios. We demonstrate that IQ designs can reduce the average duration of Phase I studies as compared to their parent designs without changing the risk-limits or MTD selection operating characteristics.  These approaches have been successfully implemented in both hematology and solid tumor Phase I studies.  

## FlexSim Health Care

Before beginning to run simulations, make sure you have registered and logged onto FlexSimHC (https://flexsim.com/clinical-trials), and downloaded the FlexSimHC module. You should also see a serial number to activate the module. To activate, go to the Help menu -> Liscence Activation, and provide the Activation ID and click Activate. 

## Run the model

Download the model named "IQdesigns" and the xlsx decision grid data provided above. 

Open up the FlexSimHC software, on the left panel, click "Open Model", select the IQ designs model you just downloaded, this step might take a while. Now on the right panel, click thee Excel icon next to the "Experiment" button and select the excel file you just downloaded and wait for the file to be imported. After that, click the "Experiment" button. 

Click the "Experiment Run" tab and customize how many replications you want, the default is 800. Click "Run Experiment". 

Now you will hear your pc fan running like it's going to explode. 

Once the experiment is complete, you have the option to export results for further analysis, just select the "DataCollector1" table under Data History Tables and click export data. 










