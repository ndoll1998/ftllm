# ft-llm
Fine-Tuning Large Language Models

This repository compares different strategies of fine-tuning large language models on numerous NLP tasks.

## structure
The directory structure follows the scheme below:
```
<TASK>/<PRETRAINED_MODEL>/<STRATEGY>
```
where `<TASK>` specifies the NLP task to solve, `<PRETRAINED_MODEL>` gives the pretrained model which is to be fine-tuned and `<STRATEGY>` is the fine-tuning strategy applied.

## reproduce
To reproduce the results first install the dependencies by running:
```bash
pip install -r requirements.txt
```

Afterwards the individual experiments can be reproduced using [`dvc`](https://dvc.org/).
```bash
dvc repro <TASK>/<PRETRAINED_MODEL>/<STRATEGY>
```

## results

Results for all tasks are presented in the corresponding directory:

 - [text classification](./text_cls)
 - [named entity recognition](./ner)
