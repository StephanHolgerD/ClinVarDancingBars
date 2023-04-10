# ClinVarDancingBars

Little repo to explain how to combine my two ClinVar repos for extracting and plotting submission informations.


## requirements
[conda env export from my working environment](condaenv.txt)


## data
- download ClinVar release of your choice
```
wget https://ftp.ncbi.nlm.nih.gov/pub/clinvar/xml/ClinVarFullRelease_00-latest.xml.gz

```


- extract gzip, if your are low on space you can also run the code directly on the .gz

```
gunzip ClinVarFullRelease_00-latest.xml.gz

```

## code



[1 - notebook for CLinVar parsing](01_ParseClinvarXML.ipynb))
- code reads in the ClinVar xml and extracts detailed infos about submissions
- runs ~ 90 minutes, depending on the number of cpu's
- outfile ~ 350mb in size

[2 - notebook for plotting](02_CreateMovingBarPlot.ipynb)
- code reads in outfile from 1. --> dataframe can be filtered for the genes and variants of interest 
- creates dict that define the single frames of the final video
- creates all the figure
- render video


## result



![](https://github.com/StephanHolgerD/ClinVarDancingBars/blob/master/movingbars.gif)

