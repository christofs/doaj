# DOAJ

Some analyses of the data published by the Directory of Open Access Journals (DOAJ). 

# APCs in Journals listed in the DOAJ 

_Christof Schöch_ (7 May 2023)

## Data 

All data comes from DOAH's public data dump: https://doaj.org/docs/public-data-dump/. 

The data was collected on January 4, 2023. It contains information about 17850 different journals. 

## Issue 

I wanted to find out what APCs are typical in OA journals, internationally. In order to be able to anwer this question, I used the information in the DOAJ dataset about APCs. The main difficulty was to convert the various currencies to one currency for comparison. I selected the EUR as the comparison currency. 

## Results 

### To APC or not to APC 

Out of the 17850 journals, 4932 (or around 28%) do charge an APC, while 12918 (or around 72%) do not. That's an interesting proportion in itself.  

### Summary statistics

The summary statistics are quite interesting, for the full data: 

* minimum: 0.0 EUR
* median: 0.0 EUR
* mean: 241 EUR
* maximum: 7938 EUR
* standard deviation: 622 EUR 

Because more than 50% of the journals do not have an APC, the median is 0 EUR! And even in DOAJ data, some journals charge more than 7000 EUR! 

And for only those 4932 journals with a non-zero APC: 

* minimum: 0.01 EUR
* median: 580 EUR
* mean: 873 EUR
* maximum: 7938 EUR
* standard deviation: 921 EUR

### The APC distribution

When looking at the full data, the histogram is of course dominated by the journals with 0 (or very very low) APC. They make up around 80% of the journals. 

![APC distribution for all journals in DOAJ](/figures/APC-histogram_all.png)

When only looking at the journals with non-zero APCs, there is still a rather dominating group of journals with very low fees, below 100 EUR. 

![APC distribution for journals in DOAJ with non-zero APCs](/figures/APC-histogram_nonzero.png)

There is also a group of around 2000 journals with APCs that one could call low, that is up to 500 EUR. Even here, they skew towards lower APCs. 

![APC distribution for journals in DOAJ with low APCs (below 500 EUR)](/figures/APC-histogram_low.png)

There is also a group of around 2000 journals with APCs that one could call "mid-range", that is between 500 and 3000 EUR. 

![APC distribution for journals in DOAJ with mid-range APCs (500-3000 EUR)](/figures/APC-histogram_midrange.png)

Finally, there is a group with high APCs, i.e. above 3000 EUR. Note that those boundaries have not been set scientifically.  

![APC distribution for journals in DOAJ with high APCs (above 3000 EUR)](/figures/APC-histogram_high.png)


### APCs by country and scientific domain  

When looking at the data from the point of view of the country of publication of a journal, clear trends emerge. 

![Percentage of journals with an APC, by country](/figures/bar_apc-per-country.png) 

In some rich countries, like the UK or Switzerland, APCs are very common. In other countries, notably in Latin America, APCs are very uncommon. Germany is somewhere in the middle, with 50% of journals having an APC. 

When looking at the data from the point of view of rough scientific domains (summarized from the DOAJ domain-related information), the trend is also very clear. 

![Percentage of journals with an APC, by scientific domain](/figures/bar_apc-per-domain.png) 

APCs are common in Science and Medicine, and uncommon in Social Sciences and Humanities. 


## Conclusion 

Most OA journals do not charge APCs at all (72%). Another 13% charge low to moderate APCs (up to 500 EUR). Yet another group, around 14%, charge mid-range APCs (between 500 and 3000 EUR). And a last, very small, group, around 0.5% (or 99 journals), charge APCs above 3000 EUR. 

APCs depend heavily on the country where the journal's publisher is located and on the scientific domain they are active in. In the Humanities, APCs are unusual (only 20% of journals have one). In the UK, more than 80% of journals have an APC.  


