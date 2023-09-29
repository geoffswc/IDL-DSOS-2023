## IDL-DSOS-2023

## Overview

This repository contains code and Jupyter workbooks for the for IDL-DSOS summer 2023 project. This project investigated the feasibility of training a machine learning model to identify which metadata tags should apply to unclassified documents in the UCSF Industry Archives Documents collection (https://www.industrydocuments.ucsf.edu). We used human-generated classification tags for a small collection for training and testing, then assessed the proper probability threshold for deciding to include or exclude a tag.

## Methods and Conclusions

For more information on this project, including methods and conclusions, please see the write up by Noel Salmeron (Summer Fellow) and Geoffrey Boushey (Head of Data Engineering).

**Evaluating Automated Transcription Accuracy: A Data Science Fellowship Report**

https://broughttolight.ucsf.edu/2023/09/22/evaluating-automated-transcription-accuracy-a-data-science-fellowship-report/

## Workbooks and Data

### data
This directory contains the .csv files (cleaned and processed from JSON output) used for analysis

### iaMetadataVideos
This directory contains the human-generated classification and tag categories for videos with existing transcripts

### json_output
This directory contains the raw json output from Google AutoML transcription for videos from the Internet Archives Collection. This information was converted into .csv output prior to analysis, processed files are available in the data directory.

### Notebook Files

The following jupyter notebooks were created by Noel Salmeron to build an ML model for each classification tag, create visuals, and analyze features.

* Classify-Advertising-Tag.ipynb
* Classify-Health-Tag.ipynb
* Classify-Lawsuit-Tag.ipynb
* Classify-News-Report-Tag.ipynb
* Classify-Opioid-Tag.ipynb
* Classify-Tobacco-Tag.ipynb

The following jupyter notebooks were created by Geoffrey Boushey to evaluate proper ML-generated probability thresholds for applying a tag to a transcript and create .csv files for analysis or prepare data for analysis. 

* Precision-Recall-Tag.ipynb
* format_json.ipynb
* file_url_list.ipynb
* Join-Transcripts-Metadata.ipynb

### Generating Transcripts

For information about the computational pipeline  used to generate transcripts from video files using google AutoML, please see the github repository for the 2023 UCTech Presentation: "Bias and Data Loss Through Transcript Generation".

https://github.com/geoffswc/UCTech-2023-Transcript-Generation










