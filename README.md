# Court Watching Data
*By Micah Clark Moody*    

### ***WELCOME!*** If you're at this repository for data on quantitative claims in my MA thesis...
_[“Bond is going to be…”: Setting and justifying pretrial conditions in Cook County Central Bond Court](https://knowledge.uchicago.edu/record/4293?ln=en&v=pdf)_ and you're not interested in the underlying code then I'd recommend going straight to [this document](https://github.com/MicahCM/bond_court/blob/main/final_paper_citations.md) for citations. If you are interested in the underlying code I would start with [this .Rmd document](https://github.com/MicahCM/bond_court/blob/main/final_paper_citations.Rmd). 

# Context on Cook County Central Bond Court

#### Overview

For context on Cook County Bond Court at the time of this research, see _["Bond is going to be..."](https://knowledge.uchicago.edu/record/4293?ln=en&v=pdf)_.

For news about current pretrial policy from advocates against money bail, see [the News page](https://endmoneybond.org/news/) from the Illinois Network for Pretrial Justice.

#### Helpful terms

- **Bond Court:** in general, when a person is arrested in Cook County, police take the arrested person to a police station. Later, everyone in the police station is taken to Cook County Jail. The first time an arrested person appears in court and is told their charges is called ***bond court*** where a judge sets conditions of supervision during the person's case. 
- **Pretrial:** the period between being accused of a crime (arrested) and found innocent, guilty, or the case being dismissed. Pretrial people are legally assumed to be innocent. Here's a [bibliography from the Vera Institute for Justice](https://www.vera.org/downloads/publications/Justice-Denied-Evidence-Brief.pdf) with more information
- **Bond:** The conditions of being released. This can mean money bail (paying money to the court with the promise part will be returned if you appear at all court dates), electronic monitoring, or even jailing. Legally, judges are supposed to assume release without any conditions is normal and anything more restrictive is unique.
- **Github:** if you're new to Github or coding in r, don't fear! The documents that end ".Rmd" will be a bit hard to follow, these are the code, but if you read `# text with a "#"` in front the steps will be explained.  

#### Types of bond and the associated money requirements:

- __I-Bond:__ Release without paying money     
  - _Example: "10,000 I" means release without paying any money_     
- __D-Bond:__ Release after paying 10% of the bond amount     
  - _Example: "10,000 D" means release after paying $1,000_      
- __C-Bond:__ Release after paying the full bond amount     
  - _Example: "10,000 C" means release after paying $10,000_     
- __No Bail:__ Refereed to generally as "no bail", the defendant is held in jail

# Repo contents

- [data_cleaned](https://github.com/MicahCM/bond_court/blob/main/data_cleaned.csv) contains court watching data. It has been unmodified, but notes and identifying information about attorneys has been removed.
- [EM Memo](https://github.com/MicahCM/bond_court/blob/main/memo_EM/memo_EM.md) is a side-project based on the EM conditions I have observed in 2022
- [final_paper_citations]() are the citations for specific quantitative claims in my MA thesis project

### Required packages
You will need these packages to run the .Rmd code and reproduce my analysis:

```
library(knitr)
library(lubridate)
library(readr)
library(tidyverse)
```
