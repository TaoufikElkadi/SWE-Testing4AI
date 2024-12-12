investigation_train_large_checked

This is the *.csv containing the data we wish you to get started with, in making your purposefully 'good' and 'bad' model.

The data uses the generator as released by Lighthouse Reports, that creates synthesized data based on the actual statistical properties of the original dataset as was used by the Rotterdam Municipality in their risk-scoring algorithm.

Each row represents the information for a synthesized Rotterdam resident. Based on the feature values (see the 'data_description.csv' file for a translation/explanation), a risk score was given to each resident, dividing a weight of 1.0 over whether a person should be checked ('ja') or not ('nee'). Effectively, this was turned into a binary prediction target ('checked') by applying a threshold on the 'ja' value. For this, we used the same threshold as was used in the original Rotterdam algorithm.

Your task is to develop both a purposefully good and bad model, that takes in data with the same features as this dataset, and then yields a binary prediction on the 'checked' column. You are free to choose whether you want to binarize this decision going through the intermediate 'ja'/'nee' scoring, or whether you straight on want to predict a binarized outcome. Furthermore, to make your model good or bad, you are welcome to adjust or resample the training data, as long as it will keep the same interface, so you can run one anothers' models without having to adjust your input reading.

In case you want to generate more or different data using the original generator, please consult https://github.com/abuszydlik/Social-Welfare-Dataset/blob/main/DataManual.md for instructions.

---

data_description

description/English translation of all feature fields