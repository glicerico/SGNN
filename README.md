# SGNN
> Implementation of Self-Governing Neural Networks for speech act classification


## Implementation of the [SGNN paper](https://www.aclweb.org/anthology/D19-1402.pdf) for speech act classification.
This repository is inspired by Guillaume Chevalier's [implementation](https://github.com/guillaume-chevalier/SGNN-Self-Governing-Neural-Networks-Projection-Layer), as well as his [discussion](https://github.com/guillaume-chevalier/SGNN-Self-Governing-Neural-Networks-Projection-Layer/issues/1) with [Sava Kalbachou](https://github.com/thinline).
This version implements some things differently from Guillaume's code, in an attempt to resemble the paper more, and extends beyond the projection layer all the way to a fully trainable network.

The network is trained to classify the [SwDA corpus](https://web.stanford.edu/~jurafsky/ws97/) utterances according to their speech act. The corpus was was pre-processed using Cristopher Pott's [project](https://github.com/cgpotts/swda/) related to it. To follow Lee & Dernoncourt SwDA data split, as in the SGNN paper, we added [adequate functionality](https://github.com/glicerico/swda/blob/data_split/create_sets.py) in our [branch](https://github.com/glicerico/swda/tree/data_split) of that repo. The pre-processed data is included in the [`data`](data) folder for repeateability.

The original SGNN paper reports a SwDA accuracy of 83.1.
With this implementation, I have only managed to achieve a maximum accuracy of 71.3; if you achieve a better score, please share your settings in an issue :)

## How to use

- Install all dependencies; use `environment.yml` file as reference.

- Open the `00_core.ipynb` notebook and modify `REPO_PATH = "<PATH-TO-SGNN-REPO>"` in the last cell. Modify any parameters you want to tweak from the network, then run the whole notebook.

- Alternatively, you can use `core.py` from the terminal or a Python IDE.

