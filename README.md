# SGNN

> Implementation of Self-Governing Neural Networks for speech act classification

## Implementation of the [SGNN paper](https://www.aclweb.org/anthology/D19-1402.pdf) for speech act classification.
This repository is inspired by Guillaume Chevalier's [implementation](https://github.com/guillaume-chevalier/SGNN-Self-Governing-Neural-Networks-Projection-Layer), as well as his [discussion](https://github.com/guillaume-chevalier/SGNN-Self-Governing-Neural-Networks-Projection-Layer/issues/1) with [Sava Kalbachou](https://github.com/thinline).
This version implements some things differently from Guillaume's code, in an attempt to resemble the paper more, and extends beyond the projection layer all the way to a fully trainable network.

The network is trained to classify the [SwDA corpus](https://web.stanford.edu/~jurafsky/ws97/) utterances according to their speech act. The corpus was was pre-processed using Cristopher Pott's [project](https://github.com/cgpotts/swda/) related to it. To follow Lee & Dernoncourt SwDA data split, as in the SGNN paper, we added [adequate functionality](https://github.com/glicerico/swda/blob/data_split/create_sets.py) in our [branch](https://github.com/glicerico/swda/tree/data_split) of that repo. The pre-processed data is included in the [`data`](data) folder for repeateability.

## How to use
See the `00_core.ipynb` notebook
