## Directory Notes
<ul>
    <li>`/output`: includes the generated labels from when we ran our model.</li>
</ul>

## Data
We found a new sarcastic data set online with more examples. The data set that was given to us had a distribution of:
75% non-sarcastic example and 25% sarcastic examples. We needed more training data for the sarcastic examples. Since the new training dataset is only 1.5mb we uploaded it to the repo as well as emailed it.

## How To Run
1. Make sure that the following directories exists:
    - `train.En.csv`
    - `task_A_En_test.csv`
2. Run the main.ipynb notebook in the root directory. By the end of this notebook a new file called `generated_labels.csv` will appear in the root directory. This file will be used as part of the input for evaluating the model using the `eval.ipynb` notebook.
3. Evaluate the model using `eval.ipynb`.