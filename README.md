# Invasive Ductal Carcinoma Classification

Image Classification for breast cancer predictions
Dataset: https://www.kaggle.com/paultimothymooney/breast-histopathology-images

Presentation: https://www.canva.com/design/DAE6T2QLFss/ruVoaJzRcIFitTn9wrUn8w/edit#

Authors: Olgert Hasko

## Overview

In situ carcinoma is "pre-invasive" carcinoma that has not yet invaded the breast tissue.  Invasive cancers have cancer cells that infiltrate outside of the normal breast lobules and ducts to grow into the breast connective tissue. Invasive carcinomas have the potential to spread to other sites of the body, such as lymph nodes or other organs, in the form of metastases.  Approximately 80% of breast carcinomas are invasive ductal carcinoma.

Source: Source: https://pathology.jhu.edu/breast/types-of-breast-cancer

-About 1 in 8 U.S. women (about 13%) will develop invasive breast cancer over the course of her lifetime

-In 2021 there were 281,550 invasive breast cancer and 49,290 in situ cases amongst women and 2,650 in men

-In 2021 43,600 deaths

-As of January 2021, there are more than 3.8 million women with a history of breast cancer in the U.S. 

-Breast cancer became the most common cancer globally as of 2021, accounting for 12% of all new annual cancer cases worldwide, according to the World Health Organization.


## Stakeholder
-Athina Breast Cancer, Albania

## The Business Problem 
Due to a shortage of qualified doctors and general corruption in thr country.  I set out to create a CNN model that would help aliviate some of the issues facing people in albania with cancer detection and follow up treatment. 

Invasive Ductal Carcinoma (IDC) is the most common subtype of all breast cancers. To assign an aggressiveness grade to a whole mount sample, pathologists typically focus on the regions which contain the IDC. As a result, one of the common pre-processing steps for automatic aggressiveness grading is to delineate the exact regions of IDC inside of a whole mount slide.

## Data & Methods
The dataset is divided into 2 folders, train_dir and val_dir, with subfolders for each picture category.  There are 198,000 clean images and 118,000 images with cancer cells.

The original dataset consisted of 162 whole mount slide images of Breast Cancer (BCa) specimens scanned at 40x. From that, 277,524 patches of size 50 x 50 were extracted (198,738 IDC negative and 78,786 IDC positive). Each patch’s file name is of the format: uxXyYclassC.png — > example 10253idx5x1351y1101class0.png . Where u is the patient ID (10253idx5), X is the x-coordinate of where this patch was cropped from, Y is the y-coordinate of where this patch was cropped from, and C indicates the class where 0 is non-IDC and 1 is IDC.



## Recommendations 

-Implement our machine learning model to assist hospitals with initial cancer detection

-Have a doctor independently review any scans with 70% or lower prediction
## Sources
https://pathology.jhu.edu/breast/types-of-breast-cancer
https://jamanetwork.com/journals/jama/fullarticle/2203798
https://www.frontiersin.org/articles/10.3389/fmed.2019.00264/full#B24
https://www.hindawi.com/journals/cmmm/2021/4019358/
https://www.charitynavigator.org/index.cfm?bay=content.view&cpid=497
https://github.com/tirthajyoti/Deep-learning-with-Python/blob/master/Notebooks/Keract-activation.ipynb

**Repository Structure:**
```
├── Model Files                            <- Files that include saved models and log files 
├── Presentation Images                    <- Images used for presentation
├── .gitignore                             <- gitignore 
├── Final_Notebook.ipynb                   <- Final notebook with best model
├── README.md                              <- The top-level README for reviewers of this project
└── tf_board_plotting.ipynb                <- Train-Validation plots for the presentation
