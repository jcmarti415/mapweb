---
layout: post
title:  "About This Project"
date:   2024-04-19 22:47:31 -0600
categories: jekyll update
---

The Colombian Armed conflict has been running for more than 60 years. In 2016 a peace process was signed between the Colombian government and the main guerrilla group, FARC-EP. The top priority of the process is to avoid more conflict, and for that, it is necessary to know the true nature of the war. All those involved in this conflict are invited to give their own point of view of the conflict, military leaders, guerrilla leaders, soldiers, victims, families, corporate owners, landlords, etc. Within this context, we have the database of the [National Security Archive][national-archive], comprised of declassified communications of the United States, from 1948 until 2009. In this paper, the diplomatic cables issued by the U.S. Embassy in Colombia from 1990 to 2009 were selected, for a total of 1009 files. Through OCR and text analysis we find that the most frequent topic in this document is the violations of human rights related to military affairs and military forces. The purpose of this project is to hel build the memory of the inner conflict in Colombia from the perspective of United States as an involved actor.

The final output of this project is a dataset that includes the locations mentioned on the 74 diplomatic cables issued in 1999 by the U.S. Embassy located in Bogota Colombia. This dataset  have information related to the location identified, such as coordinates (for digital mapping), name, country, and ISO code, among others. 

This is a proof of concept for the browsing and analysis of these documents adding a geospatial dimension. 

Tools used:

[gImage][gImageReader] for OCR 

[Mordecai][mordecai] for geoparsing

[QGIS][QGIS] for digital mapping

[Qgis2Web][qgis2web] QGIS Plugin for tinteractive maps



[national-archive]: https://nsarchive.gwu.edu/project/colombia-project
[gimagereader]:https://github.com/manisandro/gImageReader
[mordecai]:https://github.com/openeventdata/mordecai
[QGIS]: https://www.qgis.org/en/site/
[qgis2web]: https://github.com/qgis2web/qgis2web