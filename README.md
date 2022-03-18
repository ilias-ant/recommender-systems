# recommender-systems

Implementing various Recommender Systems for [Amazon review data](https://nijianmo.github.io/amazon/index.html) as well as [MovieLens](https://grouplens.org/datasets/movielens/).

This project was part of the course **Recommender Systems** at the MSc in Data Science of AUEB, carried out 
during the Winter Quarter 2021-22.

### Installation

Apart from cloning the repository, a Python interpreter (version `3.8` or greater) is also required.

```shell
python3 -m pip install poetry
```
This will install the project's dependency manager, [poetry](https://python-poetry.org/).

To install the project dependencies, type:

```shell
poetry run python -m pip install --upgrade pip
```

and then:

```shell
poetry install
```

### Reproduction

To run any available Jupyter notebook, you can do so through:

```shell
poetry run jupyter notebook
```

## Citation

For the Amazon review dataset:

```bibtex
@inproceedings{ni-etal-2019-justifying,
    title = "Justifying Recommendations using Distantly-Labeled Reviews and Fine-Grained Aspects",
    author = "Ni, Jianmo  and
      Li, Jiacheng  and
      McAuley, Julian",
    booktitle = "Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing and the 9th International Joint Conference on Natural Language Processing (EMNLP-IJCNLP)",
    month = nov,
    year = "2019",
    address = "Hong Kong, China",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/D19-1018",
    doi = "10.18653/v1/D19-1018",
    pages = "188--197",
    abstract = "Several recent works have considered the problem of generating reviews (or {`}tips{'}) as a form of explanation as to why a recommendation might match a customer{'}s interests. While promising, we demonstrate that existing approaches struggle (in terms of both quality and content) to generate justifications that are relevant to users{'} decision-making process. We seek to introduce new datasets and methods to address the recommendation justification task. In terms of data, we first propose an {`}extractive{'} approach to identify review segments which justify users{'} intentions; this approach is then used to distantly label massive review corpora and construct large-scale personalized recommendation justification datasets. In terms of generation, we are able to design two personalized generation models with this data: (1) a reference-based Seq2Seq model with aspect-planning which can generate justifications covering different aspects, and (2) an aspect-conditional masked language model which can generate diverse justifications based on templates extracted from justification histories. We conduct experiments on two real-world datasets which show that our model is capable of generating convincing and diverse justifications.",
}
```

For the Surprise library:

```bibtex
@article{Hug2020,
  doi = {10.21105/joss.02174},
  url = {https://doi.org/10.21105/joss.02174},
  year = {2020},
  publisher = {The Open Journal},
  volume = {5},
  number = {52},
  pages = {2174},
  author = {Nicolas Hug},
  title = {Surprise: A Python library for recommender systems},
  journal = {Journal of Open Source Software}
}
```

For the MovieLens dataset:

> F. Maxwell Harper and Joseph A. Konstan. 2015. The MovieLens Datasets: History and Context. ACM Transactions on Interactive Intelligent Systems (TiiS) 5, 4: 19:1–19:19. <https://doi.org/10.1145/2827872>