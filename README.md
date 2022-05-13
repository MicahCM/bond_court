# Court Watching Data
***17 Days in Cook County Bond Court from January to April, 2022***    

*By Micah Clark Moody*    

> ***WELCOME!*** This is a project under construction. Here's the timeline...
>
> - 2022-05-02: Data published
> - 2022-05-03: Brief EM memo finished
> - 2022-05-11: 2017 Order 18.8A analysis draft
> - 2022-06-04: Data analysis completed. ***This is when analysis will be edited, graphs formatted, documents published without code, and full analysis ready for critique.***
> - 2022-07-29: Final paper uploaded
> - Additional memos may be published as interesting findings emerge

### Context

- **Bond Court:** when a person is arrested in Cook County, they are taken by the police to a station to start the case and then transferred to Cook County Jail. After being jailed, they appear in *bond court* where a judge sets conditions of supervision during the person's case. People are ***assumed to be innocent*** the entire time they are under pretrial control. Here's a [bibliography from the Vera Institute for Justice](https://www.vera.org/downloads/publications/Justice-Denied-Evidence-Brief.pdf) with more information
- **Pretrial:** the period between being accused of a crime (arrested) and found innocent, guilty, or the case being dismissed. Pretrial people are assumed to be innocent.
- **Bond:** The conditions of being released. This can mean money bail (paying money to the court with the promise part will be returned if you appear at all court dates), electronic monitoring, or even jailing. Legally, judges are supposed to assume release without any conditions is normal and anything more restrictive is unique.
- **Github:** if you're new to Github or coding in r, don't fear! The documents that end ".Rmd" will be a bit hard to follow, these are the code, but if you read `# text with a "#"` in front the steps will be explained. Around or before 2022-06-04 there will be documents formatted like reports with graphs and explanation but no code in files that end `.md` 

Types of bond and the associated money requirements:

- __I-Bond:__ Release without paying money     
  - _Example: "10,000 I" means release without paying any money_     
- __D-Bond:__ Release after paying 10% of the bond amount     
  - _Example: "10,000 D" means release after paying $1,000_      
- __C-Bond:__ Release after paying the full bond amount     
  - _Example: "10,000 C" means release after paying $10,000_     
- __No Bail:__ Refereed to generally as "no bail", the defendant is held in jail 

### This project

In anticipation of the _Pretrial Fairness Act_ abolition of bail on January 1, 2023, I set out to observe bond court and interview lawyers working there. the project evolved to argue ***increase in pretrial incarceration without bail is a potential consequence of abolishing bond which requires procedural intervention in addition to legal safeguards.*** To reach this conclusion, I have built on the work of the _Coalition to End Money Bond_ and _Appleseed Center for Fair Court's_ excellent 2017 court watching effort and analysis of a policy change that diminished the use of bond. To develop context on the current bond court process, I conducted qualitative analysis and interviews in addition to this quantitative overview.

> Questions, data requests, and concerns: contact Micah Clark Moody at michaclarkmoody@gmail.com

# Repo contents

- [data_cleaned](https://github.com/MicahCM/bond_court/blob/main/data_cleaned.csv) contains court watching data. It has been unmodified, but notes and identifying information about attorneys has been removed.
- [2022_data_analysis](https://github.com/MicahCM/bond_court/blob/main/2022_data_analysis.Rmd) has the code for analyzing the 2022 courtwatching data
- [2017_data_analysis](https://github.com/MicahCM/bond_court/blob/main/2017_data_analysis.Rmd) has the code for analyzing the 2017 courtwatching data collected by the Coalition to End Money Bond
- [EM Memo](https://github.com/MicahCM/bond_court/blob/main/memo_EM/memo_EM.md) is a side-project based on the EM conditions I have observed in 2022

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

The 2017 data was collected by volunteer court watchers coordinated by the Coalition to End Money Bond. Their methods are available [here](https://gitlab.com/ChicagoDataCooperative/court-observation/-/blob/master/data_processing.Rmd).

### Limitations
The 2017 courtwatching data is relatively comprehensive. 

There are several important limitations to the 2022 courtwatching data.

- _Inconsistent watching_
- _Uneven coverage of judges_
- _Over representation of weekend calls_
- _Over representation of call beginnings_ 
