# Statistics for Gaza's Coronavirus outbreak
This repository contains statistics for the outbreak of coronavirus in Gaza.
These statistics are taken from official daily Ministry of Health reports. You
can find these reports manually transcribed into the document spreadsheet.

These documents are released as Creative Commons By Attribution ShareAlike

The ministry does not release daily reports any more as far as I can tell. You can find daily statistics [at their official site](https://www.moh.gov.ps/portal/coronavirus)

# Conversion regex
To convert the names of the Ministry-issued reports to ISO formatted dates, I use the `rename` command:
```
sudo apt install rename
rename 's/Cor.\ Eng\ (.*)-(.*).pdf/2021-$2-$1.pdf/' *.pdf
rename 's/Cor.\ Eng\.(.*)-(.*).pdf/2021-$2-$1.pdf/' *.pdf
rename 's/Cor.\ Eng\ (.*)\.(.*).pdf/2021-$2-$1.pdf/' *.pdf
rename 's/Cor.\ Arab-Eng\ (.*)\.(.*).pdf/2021-$2-$1.pdf/' *.pdf
```
