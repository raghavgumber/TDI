# TDI
## Analysis Overview:
There are plenty of sources (SBA-Small Business Administration being one of them) that provide abundant loan level information. We look at SBA data (which aims to provide guarantees on loans made to small businesses, in hopes to encourage lending by Banks). I propose that by looking at loan level data, we can actually come up with a metric to predict what is the "loss rate" in the market. This should hopefully aim to provide a benchmark for the strength of the small business loan market.

To get a metric of loan performance of all existing loans in the universe, we implement an open pool loss rate calculation. The open pool approach is a non-cohort approach in which charge-offs are tracked over a period of time, with no tracking of activity or balances of specific loans. We essentially assume our pool of loans starts getting originated from 1991 (when SBA data starts becoming available) and all loans in pool stay in the pool until paid off or charged off. 

As of now, I only try to look at whether I can come up with some empirical analysis to arrive at an estimate of the loss rate of loans in the small business market in presence of a credit bust. This is as I particularly focus on performance of the loan market around 2008 (2007-12 to 2011-06). This ofcourse still needs to take all loans in to account up to 2008. I further try to see if I can use my empirical analysis to have an estimate for another period of time (in this case, the Oil crash of 2014/15).

### Data:
- SBA Data is pulled via SBA website that includes loans made from 1991 forward guaranteed (partially) by the SBA. (https://www.sba.gov/about-sba/sba-performance/open-government/foia/frequently-requested-records/sba-7a-504-loan-data-reports)
- Macroeconomic level data dealing with unemployment rates by different states and Bank Prime rate since 1991 is pulled via FRED API. (If you do not have this, please install)

### Code:
lossRateIndependentProject.jpynb contains all the code that is self-contained and can be used to reproduce all the analysis done herein.

### Report:
A Detailed report is also attached
