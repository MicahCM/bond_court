# Court Watching Data
***17 Days in Cook County Bond Court from January to April, 2022*** <br>
<br>
*By Micah Clark Moody*

### Context

- Bond Court
- Pretrial
- Bond
- Github: if you're new to Github or coding in r, don't fear! The documents that end ".Rmd" will be a bit hard to follow, these are the code, but if you read text with a "#" in front of it the steps should be explained. Around or before 2022-06-04 there will be documents formatted like reports with the graphs but without the code that will be more accessible. 

> __I-Bond:__ Release without paying money     
> _Example: "10,000 I" means release without paying any money_     
> __D-Bond:__ Release after paying 10% of the bond amount     
> _Example: "10,000 D" means release after paying $1,000_      
> __C-Bond:__ Release after paying the full bond amount     
> _Example: "10,000 C" means release after paying $10,000_     
> __No Bail:__ Refereed to generally as "no bail", the defendant is held in jail 

### This project

In anticipation of the _Pretrial Fairness Act_ abolition of bail on January 1, 2023, I set out to observe bond court and interview lawyers working there. the project evolved to argue ***increase in pretrial incarceration without bail is a potential consequence of abolishing bond which requires procedural intervention in addition to legal safeguards.*** To reach this conclusion, I have built on the work of the _Coalition to End Money Bond_ and _Appleseed Center for Fair Court's_ excellent 2017 court watching effort and analysis of a policy change that diminished the use of bond. To develop context on the current bond court process, I conducted qualitative analysis and interviews in addition to this quantitative overview.

> Questions, data requests, and concerns: contact Micah Clark Moody at michaclarkmoody@gmail.com

# Repo contents

- [data_cleaned](https://github.com/MicahCM/bond_court/blob/main/data_cleaned.csv) contains court watching data. It has been unmodified, but notes and identifying information about attorneys has been removed.
- [2022_data_analysis](https://github.com/MicahCM/bond_court/blob/main/2022_data_analysis.Rmd) has the code for analyzing the 2022 courtwatching data
- CLEAN COPY
- [2017_data_analysis](https://github.com/MicahCM/bond_court/blob/main/2017_data_analysis.Rmd) has the code for analyzing the 2017 courtwatching data collected by the Coalition to End Money Bond
- CLEAN COPY
- FINAL PAPER
- EM Memo

### Required packages
You will need these packages to run the .Rmd code and reproduce my analysis:

```
library(knitr)
library(lubridate)
library(readr)
library(tidyverse)
```

### Methods
To collect the 2022 data, I listened to the audio stream of court on YouTube. On two dates, # and #, I watched court over zoom and could visually defendants. # and # are thus the only dates that I could record 'apparent_race'.

The 2017 data was collected by volunteer court watchers coordinated by the Coalition to End Money Bond. Their methods are available [here]().

### Limitations
The 2017 courtwatching data is relatively comprehensive. 

There are several important limitations to the 2022 courtwatching data.

- _Inconsistent watching:_
- _Uneven coverage of judges:_
- _Over representation of weekend calls:_
- _Over representation of call beginnings:_ 

### Timeline

1. 2022-05-02: Data published
1. 2022-06-04: Data analysis completed, format as accessible documents, graphs will be labled and pretty
1. 2022-07-29: Final paper uploaded
1. Additional memos may be published as interesting findings emerge

# Learn more about bond

- 

### Sources

_For EM charts_
- [List of non-probationable offenses](https://illinoiscaselaw.com/sentencing-index/)