# Arabic Dialect Identification
## Used Datasets:
 - [NADI 2020 (The First Nuanced Arabic Dialect Identification Shared Task)](https://github.com/UBC-NLP/nadi)
 - [QCRI Arabic Dialect Identification (QADI)](https://github.com/qcri/QADI)
 - Download the QADI processed dataset [link](https://drive.google.com/file/d/1-4EVHyvmaJLao6WLqYYifVIprhQgihi3/view?usp=share_link)

## The [QADI-Experiments](https://github.com/bioengsamar/Arabic-Dialect-Classification/tree/main/QADI-Experiments) & [QADI-Experiments](https://github.com/bioengsamar/Arabic-Dialect-Classification/tree/main/NADI-Experiments) folders contain the base model (AraBERT), bert-base-arabertv02-twitter, MARBERTv2 and finally Ensemble approach training and testing 
## Results 
 - Results and findings of the Solving the First Nuanced Arabic Dialect Identification Shared Task (NADI), Subtask 1 (country level dialect identification):
 
Model | F1 |ACC | Epochs | SEQ-LEN
------ |------|-----|------|----| 
Base Model |26 %|43.7 %| 3 | 80
Ensemble Base Model |29.03 %|45.07 %| - | -
bert-base-arabertv02-twitter | 29.015 %|  46.52 % | 4 | 80
MARBERTv2 | 29.504 %| 48.45 % | 4 | 80
**Ensemble Model**| **31.477 %**| **50.11 %** | - | -


 - Results and findings on the second dataset (QADI):

Model | F1 |ACC | Epochs | SEQ-LEN
------ |------|-----|------|----| 
Base Model |46.90 %|50.28 %| 6 | 80
bert-base-arabertv02-twitter | 54.93 %| 57.26 % | 6 | 80
MARBERTv2 | 56.31 %| 58.83 %| 6 | 80
Ensemble Model | 58.80 % |  61.11 % | - | -
---------------------
