# Important Documents

`hotpot_dev_fullwiki_v1.json`: questions used for evaluation

`HotpotQA Wikipedia corpus`: used by RAG system to retrieve documents (used as context for question)

`hotpot_evaluate_v1.py`: reads the system's predictions and the dev set’s correct answers. It compares them and prints the scores.

`project.ipynb`: our custom system used to generate predictions for questions from `hotpot_evaluate_v1.py`

# About the system

After running the system on the dev set the output should be a JSON file of all the predictions, one for each question.

The prediction needs to be formatted according to the Dev example provided on
the HotPotQA webpage: https://hotpotqa.github.io/

# How to run the eval script

1. `pip install ujson`
2. `python hotpot_evaluate_v1.py <Your JSON prediction file> hotpot_dev_fullwiki_v1.json`
