First, install xgboost first via
```
pip install xgboost
```

To run BOW.ipynb
- First, update data_folder_path to match path to two csv files
- Second, update countvec_path to match path to your countvec.npz files
- Third, to run Dimension Reduction cell, be careful of RAM overload, I encounter this on Google Colab. It is recommended to run each part of the following cell once after reset variables to avoid RAM overload
- Last, to export my submission csv to Kaggle, update path of output csv file in function export_kaggle. This will export csv file of Logistic Regression model

To run doc2vec.ipynb
- First, update data_folder_path to match path to two csv files
- Second, since our model use doc2vec with 400 size vector. Please rerun genism code, update vector size to 400. We only need train set for validating. Put three output files to the same folder
- Third, update filename to the following variables train_ingre_doc2vec100_filename, train_steps_doc2vec100_filename, train_name_doc2vec100_filename. Update doc2vec100_path to path contain your three output files
- If you want to evaluate performance against different doc2vec vector, please export doc2vec embedding corresponding to vector size first, then update filename in each cells. However this is realy time consuming
- If you have tested with diffrent doc2vec embedding, please load doc2vec400 again, to the follwing variable train_ingre_doc2vec100_filename, train_steps_doc2vec100_filename, train_name_doc2vec100_filename BEFORE training model

To run Select Training Size.ipynb
- First, update data_folder_path to match path to two csv files
- Second, update filename to the following variables train_ingre_doc2vec100_filename, train_steps_doc2vec100_filename, train_name_doc2vec100_filename. Update doc2vec100_path to path contain your three output files

To run metadata.ipynb
update data_folder_path to match path to two csv files

Result for all model shoudld appear under each cell, install jupyter extrension on vscode or open these notebooks in colab