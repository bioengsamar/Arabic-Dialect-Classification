# Arabic Dialect Identification
 - Our Proposed System
 ![](pipe.png)
## Used Datasets:
 - [NADI 2020 (The First Nuanced Arabic Dialect Identification Shared Task)](https://github.com/UBC-NLP/nadi)
 - [QCRI Arabic Dialect Identification (QADI)](https://github.com/qcri/QADI)
 - Download the QADI processed dataset [link](https://drive.google.com/file/d/1-4EVHyvmaJLao6WLqYYifVIprhQgihi3/view?usp=share_link)

## How to Reproduce/Run the code:
 - [Download_QADI_dataset Notebook](https://github.com/bioengsamar/Arabic-Dialect-Classification/blob/main/Download_QADI_dataset.ipynb) indicates how to download the QADI dataset using [twarc library](https://github.com/alblaine/twarc-tutorial/blob/master/README.md) 
 - [Data_Preprocessing Notebook](https://github.com/bioengsamar/Arabic-Dialect-Classification/blob/main/Data_Preprocessing.ipynb) contains the Arabic tweet Preprocessing steps using [PyArabic Package](https://github.com/linuxscout/pyarabic)
 - The [QADI-Experiments](https://github.com/bioengsamar/Arabic-Dialect-Classification/tree/main/QADI-Experiments) & [NADI-Experiments](https://github.com/bioengsamar/Arabic-Dialect-Classification/tree/main/NADI-Experiments) folders contain the base model (AraBERT), bert-base-arabertv02-twitter, MARBERTv2 and finally Ensemble approach training and testing 
 


## Results 
 - Results and findings of the Solving the First Nuanced Arabic Dialect Identification Shared Task (NADI), Subtask 1 (country level dialect identification):
 
Model | F1 |ACC | Epochs | SEQ-LEN
------ |------|-----|------|----| 
Base Model |26 %|43.7 %| 3 | 80
Ensemble Base Model |29.03 %|45.07 %| 3 | 80
bert-base-arabertv02-twitter | 29.015 %|  46.52 % | 4 | 80
MARBERTv2 | 29.504 %| 48.45 % | 4 | 80
**Proposed Ensemble Model**| **31.477 %**| **50.11 %** | **4**| **80**


 - Results and findings on the second dataset (QADI):

Model | F1 |ACC | Epochs | SEQ-LEN
------ |------|-----|------|----| 
Base Model |46.90 %|50.28 %| 6 | 80
bert-base-arabertv02-twitter | 54.93 %| 57.26 % | 6 | 80
MARBERTv2 | 56.31 %| 58.83 %| 6 | 80
**Proposed Ensemble Model** | **58.80 %**|  **61.11 %**| **6**| **80**

 - Results and findings on the second dataset (QADI) when changing the max length during AraBERT training

F1 |ACC | # Samples | Epochs | SEQ-LEN
------|-----|------|----|----| 
47.5 %|52.3 %|100k|6 | 113
52.44 %| 55.04 %| All Data| 6 | 113
54.22 %| 57 %| All Data| 10|32
---------------------
