# Statistics for Gaza's 2020 Coronavirus outbreak
This repository contains statistics for the 2020 outbreak of coronavirus in Gaza.
These statistics are taken from official daily Ministry of Health reports. You
can find these reports manually transcribed into the document spreadsheet.

These documents are released as Creative Commons By Attribution ShareAlike

# Conversion regex
To convert the names of the Ministry-issued reports to ISO formatted dates, I use the regex:
Find: ```Cor.%20Eng%20(.*)-(.*)```
Replace: ```Cor.%20Eng%20\1-\2 2020-\2-\1.pdf```
