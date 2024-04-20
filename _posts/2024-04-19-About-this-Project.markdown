---
layout: post
title:  "Dataset creation"
date:   2024-04-19 22:47:31 -0600
categories: jekyll update
---


The documents stored by DNSA are PDF files comprised of scanned images of the original print. Therefore, the text needs to be digitized, for this open-source software is used to do OCR. Due to the limitations of OCR technology, the quality of the original files and because some parts are redacted, the initial output of the software needs to be verified and improved. This was done manually to avoid losing important information.

For the identification of the location within the text, a Python library called [Mordecai][mordecai] was used. This module requires using a docker container and an index created based on the Geonames.org gazetteer. The library is well documented, and it needs a good amount of modification to be able to run locally. Other alternatives were considered; however, Python allows for better adaptation of the library to the project needs.

After obtaining the locations, words related to killing, kidnapping and drugs were counted by location and document, allowing to see how certain territories are mentioned around these topics. Any other crime related word such as violence, assaults or stealing are on the “other” category.

The dataset is comprised of 185 rows and 59 columns. Each observation is a unique combination of locaiton and document name. The other columns includes coordinates, date of the document, word counting, country ISO code, among others. 

This were joined and summarized by country and by colombian deparment using QGIS. With this two choroplets maps were created and two time sequences. 

Limitations

It is likely that these are not all the documents issued by the U.S. Embassy on 1999, wich makes difficult obtain a complete image of the country interests. Nevertheless it is stills a valuable historic source.

The quality of the images, limitaitons on COR tehcnology and geolocalization also have to be considered. 

Non-official locations, such as those named by locals only, might not be detected becase are not included on the Geonames Gazeteer. 

Some locations can get linked to unrelated events (words) becuase of the methods used.








[mordecai]:https://github.com/openeventdata/mordecai
