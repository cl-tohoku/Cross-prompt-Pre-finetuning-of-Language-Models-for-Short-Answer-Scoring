# Reducing_cost

This repository includes scrpits for a paper titled: Cross-prompt-Pre-finetuning-of-Language-Models-for-Short-Answer-Scoring (to be appear) extended version of [this paper](https://link.springer.com/chapter/10.1007/978-3-031-36272-9_7) . 

There are three function in the main script.
1. **Training**: Fine-tuning a model for specific prompt based on a given configuration.
2. **Evaluation**: Evaluating the fine-tuned model on a test dataset
3. **Zero-shot Evaluation**: Evaluating the model without further fine-tuning.

## Installation

> pip install -r requirement.txt

##Usage
### Training
#### BERT
To train a model for a specific prompt with a conf file:
> python main.py train --config_path <path_to_config>

#### LLM
WIP

### Evaluation
To evaluate the fine-tuned model on a test dataset from a specific prompt:
>python main.py eval --config_path <path_to_config> [--test_path <path_to_test_data>] [--save_path <path_to_save_results>] [--prompt <prompt_id>] [--item <item_id>]

#### LLM
WIP


### Zero-shot evaluation
>python main.py eval_zero --config_path <path_to_config> --save_path <path_to_save_results>

#### LLM
WIP


### Data set
The dataset is available for academic use through the following link: https://www.nii.ac.jp/dsc/idr/rdata/RIKEN-SAA/
To use this scripts, you need to convert the json file to tsv file with three columns: answer, criteria and score.


