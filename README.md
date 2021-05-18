# OCR_Pipeline_Results
https://www.openu.ac.il/en/omilab

We present here a corpus of 19th century Hebrew newspapers which was created at OMILab, The Open Media and Information Lab at the Open University, Israel. OmiLab’s project on Historical Newspaper Archive Research ran in collaboration with the National Library of Israel, that provided access to selected image and OCR output files at the back end of JPRESS - the Historical Jewish Press collection of the Tel Aviv University and the National Library of Israel. 

Worldwide, large historical newspapers digitization project provide oceans of valuable historical periodical data. Much of this data, however, is available in platforms that provide mediocre OCR, which hinders the application of text analytical methods of distant reading, NLP, NER and various methods of semantic processing. In order to overcome this obstacle we used the platform Transkribus to train a model for historical Hebrew print, improving significantly both line detection and character recognition. In order not to lose the valuable work that was done to analyze the layout and content structure of the newspapers we created an open workflow which migrates legacy segmentation data into the open Page format, on which the improved text recognition technologies can run, and then outputs the data as a TEI-XML encoded and enriched corpus.

## The format of the files:

### *CSV by Article:*
this folder contains a sub folder for each of the newspapers in our corpus. In each sub folder are to be found a file for each available issue of the newspaper, presented as comma separated values. Each row in the file contains an Article id, headline, and the text. 
(notice that the OCR of headlines is often problematic and worse that the text of the article).
The article ID itself contains important metadata on the article: it starts with the newspaper code and the date of publication, and ends with article id and the number of the article in the table of content (e.g. "toc_3") relative to the other articles in the issue.  
021-HLB-1874-01-07-PG001-SINGLE-ORIGNAME_100355_toc_1	

### *Plain texts:*
Each newspaper folder contains
