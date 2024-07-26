# VulFed
An FL-based Vulnerability Detection Framework.

## How to Use VulFed?

## Dataset
To run a complete framework, you need to prepare three types of data (or other extensions that can be input into LLM or GNN models in the same format). In our paper, We use raw codes, code gadgets, and SeVCs. Please refer to [[link]](https://proceedings.neurips.cc/paper_files/paper/2019/hash/49265d2447bc3bbfe9e76306ce40a31f-Abstract.html), [[link]](https://ieeexplore.ieee.org/abstract/document/9321538), and [[link]](https://arxiv.org/abs/1801.01681#) for data preparation.

## Model
All LLMs used by VulFed are pre-trained versions. When you want to use the LLM option, you must install the corresponding LLM version in advance. After installation, configure the option '-- datapath' as the root directory for storing pre training parameters. The model versions we use are BERT-base, CodeBERT-base, GPT-2-small, OPT-small, T5-small, and CodeT5-small. To obtain these pre-training parameters, please refer to [[link]](https://huggingface.co/models).

## Option
In addition to the model, we have also prepared multiple dimensions of options, including input data format, PEFT training strategy, and FL algorithm. It is recommended to run this framework through launching main.py using the command line. For specific configuration methods, please refer to the detailed notes on selectable options in the options.py located in the root directory.
