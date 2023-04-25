# sarcasm-detector

Abu Farha, I., Oprea, S. V., Wilson, S., & Magdy, W. (2022). SemEval-2022 Task 6: iSarcasmEval, Intended Sarcasm Detection in English and Arabic. In Proceedings of the 16th International Workshop on Semantic Evaluation (SemEval-2022) (pp. 802-814). Association for Computational Linguistics.

---

## How to run
### (1) Open a Google Colab session
Open a new Google Colab session and upload the following files:
* `main.ipynb`: this is the file where the model is created, trained and where the weights are found.
* `evaluation.ipynb`: this is the file where the model evaluates the generated test labels against the original test labels.
* `data`: contains the training and test data for the model.

### (2) Run `main.ipynb`
Run the two cells in `main.ipynb`. Once the second cell completes, two files should be generated in the directory that the `main.ipynb` file lives:
* `saved_weights.pt`: this is where the model's weights are stored during training.
* `generated_labels.csv`: this contains the generated labels for the test file. this is the file that will be used as an input for the `evaluation.ipynb` file.

### (3) Run `evaluation.ipynb`
Make sure that the files `data/test/task_A_En_test.csv` and `generated_labels.csv` exist in the directory where the `evaluation.ipynb` notebook lives. This notebook will output how well the model did.

## **Important To Note**
* It is expected that the training and test data are in the same format that was given.
* Our results were obtained in a Google Colab environment where it is possible to set the runtime type to GPUs to increase the speed of training over epochs.