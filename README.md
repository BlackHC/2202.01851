# Repository for ['A Note on "Assessing Generalization of SGD via Disagreement"'](https://arxiv.org/abs/2202.01851)

> Several recent works find empirically that the average test error of deep neural networks can be estimated via the prediction disagreement of models, which does not require labels. In particular, Jiang et al. (2022) show for the disagreement between two separately trained networks that this `Generalization Disagreement Equality' follows from the well-calibrated nature of deep ensembles under the notion of a proposed `class-aggregated calibration.' In this reproduction, we show that the suggested theory might be impractical because a deep ensemble's calibration can deteriorate as prediction disagreement increases, which is precisely when the coupling of test error and disagreement is of interest, while labels are needed to estimate the calibration on new datasets. Further, we simplify the theoretical statements and proofs, showing them to be straightforward within a probabilistic context, unlike the original hypothesis space view employed by Jiang et al. (2022).

See https://arxiv.org/abs/2202.01851

## Citation

> Kirsch, Andreas, and Yarin Gal. "A Note on" Assessing Generalization of SGD via Disagreement"." arXiv preprint arXiv:2202.01851 (2022).

BibTeX:

```bibtex
@misc{kirsch2022note,
    title={A Note on "Assessing Generalization of SGD via Disagreement"},
    author={Andreas Kirsch and Yarin Gal},
    year={2022},
    eprint={2202.01851},
    archivePrefix={arXiv},
    primaryClass={cs.LG}
}
```

## Reproduction

In this repository, we provide the code to reproduce the results of the paper. We load pre-trained models from [timm](https://github.com/rwightman/pytorch-image-models) and evaluate them on
ImageNet and PACS. To train the WRN models for CIFAR-10, see https://github.com/omegafragger/DDU.

### Setup

```
pip install timm
pip install hub
pip install blackhc.project
pip install tqdm
```

