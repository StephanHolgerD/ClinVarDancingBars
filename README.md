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

![](https://github.com/StephanHolgerD/ClinVarDancingBars/blob/master/movingbars.gif)

