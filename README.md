# A Hebrew 19th century press corpus

We present here a corpus of 19th century Hebrew newspapers which was created at OMILab, The Open Media and Information Lab at the Open University, Israel. 
[OmiLab’s project on Historical Newspaper Archive Research](https://www.openu.ac.il/en/omilab/pages/historicalnewspaper.aspx) ran in collaboration with the [Historical Jewish Press project](https://web.nli.org.il/sites/JPress/English) of the Tel Aviv University and the National Library of Israel.  [The National Library of Israel] (https://web.nli.org.il/sites/nli/english/pages/default.aspx) provided access to selected image and OCR output files at the back end of JPRESS. 

Worldwide, large historical newspapers digitization project provide oceans of valuable historical periodical data. Much of this data, however, is available in platforms that provide mediocre OCR, which hinders the application of text analytical methods of distant reading, NLP, NER and various methods of semantic processing. In order to overcome this obstacle we used the platform Transkribus to train a model for historical Hebrew print, improving significantly both line detection and character recognition. In order not to lose the valuable work that was done to analyze the layout and content structure of the newspapers we created an open workflow which migrates legacy segmentation data into the open Page format, on which the improved text recognition technologies can run, and then outputs the data as a TEI-XML encoded and enriched corpus.

The corpus is also indexed and made available  through the [he-story search engine] (https://www.openu.ac.il/he-story/index.html#/)

For more information about the project and the pipeline, see 

For more information about the Newspapers, browsing and searching of the scanned issues:
[The Lebanon⁩ - ⁨הלבנון⁩⁩; מכתב עתי בשפת עבר](https://www.nli.org.il/en/newspapers/hlb)
[HaCefira⁩ - ⁨הצפירה⁩⁩; מכתב עתי משמיע חדשות](https://www.nli.org.il/en/newspapers/hzf)
[HaMelitz⁩ - ⁨המליץ⁩⁩; בין עם ישרון והממשלה, בין האמונה וההשכלה](https://www.nli.org.il/en/newspapers/hmz)
[HaMagid⁩ - ⁨המגיד⁩⁩; מכתב עתי לכל עניני ישראל](https://www.nli.org.il/en/newspapers/mgd)
[Habazeleth⁩ - חבצלת](https://www.nli.org.il/en/newspapers/hzt)


## The format of the files:

### *CSV by Article:*
this folder contains a sub folder for each of the newspapers in our corpus. In each sub folder are to be found a file for each available issue of the newspaper, presented as comma separated values. Each row in the file contains an Article id, headline, and the text. 
(notice that the OCR of headlines is often problematic and worse that the text of the article).
The article ID itself contains important metadata on the article: it starts with the newspaper code and the date of publication, and ends with the issue unique ID and then the number of the article in the table of content (e.g. "toc_3") relative to the other articles in the issue.  

### *Plain texts:*
Each newspaper folder contains plain text files, one file represents an entire issue. The naming of the files includes the newspaper code, the date of publication and the issue ID. 

## License
<img src="https://github.com/yanirmr/historical_press/blob/master/OCR_Pipeline/images_for_tutorial/CC-BY-SA_icon.svg.png" width="200" height="50" />

The code is licensed under a [Creative Commons Attribution-Share Alike 3.0](https://creativecommons.org/licenses/by-sa/4.0/). You are welcome to copy and redistribute the material in any medium or format, remix, transform, and build upon the material for any purpose, even commercially,  as long as you give appropriate credit to OMILab, provide a link to the license,  indicate if changes were made and distribute your contributions under the same license as the original. 
