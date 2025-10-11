# DS-Fake-News-Project
Second semester project in data science 


# Guidelines for processing of code
First, create a fresh virtual environment or make sure your existing environment does not contain conflicting packages. Next, run `pip install -r requirements.txt` to install all necessary libraries. The `requirements.txt` file includes the packages scikit-learn, nltk, and seaborn, which will automatically pull in their dependencies if they are not already present. This ensures you have a clean, consistent setup to run the code without conflicts.

Ensure that your working directory is empty to avoid any filename conflicts. Then, download the GitHub repository.

## PART 1
- First, download the sample version of the FakeNewsCorpus and save it as `news_sample.csv`. Then, download the complete dataset and save it as `995,000_rows.csv`.
- After that, download the Jupyter Notebook `PART1_final.ipynb` from the `DS-Fake-News-Project/Part 1/` folder on GitHub and run it sequentially as arranged.
    - Make sure files named `cleaned_file.csv` , `X_train`, `X_test,` and `X_val` are not already present in your directory. 

## PART 2
- Once completed, ensure that your working directory contains the files `cleaned_file.csv` and `output_big.txt` – downloaded from the GitHub repository.
- After confirming these files are present, proceed by executing the cells in `Part 2/Task_0_1_2_3` followed by those in `Part 2/More_exploration.ipynb`.

## PART 3
- Ensure that you have executed all the files in Part 1 so that the files  `X_train` and `X_test,` are generated in your working directory, and verify that it is located in the same directory as - `AdvancedPart3_final.ipynb`.
- Execute `AdvancedPart3_final.ipynb` in sequential order—either by clicking each code cell or using the `Run All` option—to run the script as intended.

## PART 4
- Download the LIAR dataset and ensure that the file `test.tsv` is in your working directory.
- Before running the cells in `Part 4/Task_1_2_3_simple_model.ipynb`, verify that you have executed all previous parts. This should result in a file named `WITHOUT_NUM_cleaned_file_with_labels.csv` being present in your working directory.
