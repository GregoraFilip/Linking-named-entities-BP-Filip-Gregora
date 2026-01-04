# Linking named entities extracted from Czech biomedical texts with standard vocabularies
by Filip Gregora

## Description
This project is part of a bachelor thesis called Linking named entities extracted from biomedical texts with standard vocabularies written by Filip Gregora. The thesis can be accessed at: [https://is.muni.cz/auth/th/s4icj/](https://is.muni.cz/th/s4icj/).

### Abstract
We can achieve faster and more accurate medical decision-making thanks to machine learning methods in healthcare. Unfortunately, most medical information is stored in unstructured text, which is unsuitable for machine learning methods. As a solution, this work implements a technique that connects named entities obtained from Czech biomedical texts with standard dictionaries. This technique works in three steps. The first step is generating candidate entities from standard dictionaries. The second step is ranking candidate entities and selecting the best-rated candidate entity. The third step is recognizing unlinkable entities and replacing them with NIL values. This work uses a dataset designed for named entity recognition, from which a dataset on which the technique is evaluated is created.

## Technologies
The project is written in Python and is in the form of a jupyter notebook. Necessary libraries are in **requirements.txt**.

## Run
To run the project you need to:
1. Install requirements listed in file **requirements.txt**
2. Obtain a dataset of mentions from patient reports
3. Obtain a dataset of evaluated mentions
4. Obtain databases: [MSHCZ](https://nlk.cz/pro-knihovny/data), [DLP by SUKL](https://opendata.sukl.cz/?q=katalog/databaze-lecivych-pripravku-dlp), [DrugBank](https://go.drugbank.com/releases/latest)
5. Run Jupyter notebook
6. Run **NEL.ipynb**, file where is implemented technique
7. Run **evaluate_NEL.ipynb** to evaluate linking.

## File Structure
- **NEL.ipynb** is file with implemented technique.
- **evaluate_NEL** is file used for evaluating linking.
- In folder **exploratory_analysis** there are notebooks used for experimenting and playing with implemented technique.
- In folder **exploring_dataset** there are notebooks used for exploring datasets and generating statistics about them.
- In folder **preprocessing** there are notebooks for preprocessing databases.

