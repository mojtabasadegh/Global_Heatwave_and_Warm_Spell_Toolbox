# Global_Heatwave_and_Warm_Spell_Toolbox
This toolbox calculates, based on different definitions of the literature, and plots different characteristics of heatwaves/warm-spells for any country around the globe and plots the results. HW characteristics include, number of events, number of HW days, first and last HW day of year, HW magnitude, HW amplitude etc.

GHWT is a user-friendly and flexible toolbox developed in MATLAB to construct long term heatwave and warm-spell record with any gridded global daily temperature data source for any country around the globe. The user can select to perform computations using either the graphical user interface (GUI; execute "GHWT.m" in MATLAB) or  the "run script" (modify and execute "GHWT\_Script\_run.m" in MATLAB). First step is to select temperature data source and the country (or continent) for the analysis. 
This first step is designed for the CPC temperature data source. If the user opts to employ any other source for temperature data, 
(s)he should first modify the "config.txt" file and execute "extract_data.m" under the "extract other database format" subforlder to pre-process the source data. 
Subsequent steps can all be performed in the GUI. Next is to select the heatwave/warm-spell identification method, and selection of data type  (max, min, or average daily temperature). Subsequently, the user should define the method-specific parameters of the analysis (such as the number of consecutive days  for the temperature to be above a certain threshold). If the user selects the "Summer method", (s)he needs to define the start and end date of summer. The user then  selects the start and end year of analysis and execute the program. The GHWT toolbox plots several figures displaying the number of heatwave days and events,  first and last heatwave day, length of longest heatwave, and magnitude and amplitude of heatwaves for each year. These information will also be saved under  "GHWT_results.mat" under the "result" folder.
