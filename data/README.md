# Datasets

## Elon Musk's tweets

A set of tweets from Elon Musk.

Download from: https://query.data.world/s/i63ntyye4lzdjb3sfeor4ex7labc5j

Source: https://data.world/adamhelsinger/elon-musk-tweets-until-4-6-17

```
import pandas as pd
df = pd.read_csv('https://query.data.world/s/i63ntyye4lzdjb3sfeor4ex7labc5j')
```

Also see (for more Twitter datasets): https://github.com/shaypal5/awesome-twitter-data

## British Library 19th century books

A set of 452 books (their first volume) from the British Library, (mostly from the) 19th century.

Source: https://data.bl.uk/digbks

The extra metadata with book type and genre information was kindly made available by Christin Hoene <C.Hoene@kent.ac.uk>.

### Contents

* [Sample dataset folder](bl_books/sample) with:
    - [Catalog metadata](bl_books/sample/book_data_sample.json)
    - [Enriched metadata](bl_books/sample/data/bl_books/sample/extra_metadatasample.csv)
    - [Fulltext files](bl_books/sample/full_texts)
* [Sample tidy dataset folder](bl_books/sample_tidy) this is the tidy version of the sample dataset. We create it as part of class 2.1. It includes:
    - [book dataframe](bl_books/sample_tidy/df_book.csv)
    - [book_text dataframe](bl_books/sample_tidy/df_book_text.csv)
    - [author dataframe](bl_books/sample_tidy/df_author.csv)
    - [author-book dataframe](bl_books/sample_tidy/df_author_book.csv)
* [Original metadata (compressed)](bl_books/book_metadata.zip) contains catalog metadata for every book in the full dataset.
* [Original enriched metadata (csv)](bl_books/data/bl_books/sample/extra_metadata_sample.csv) contains the enriched metadata for every book in the full dataset (amnd more).
* [Original enriched metadata (xls)](bl_books/data/bl_books/sample/extra_metadata_sample.xls) contains the enriched metadata for every book in the full dataset (amnd more).

### How we created the sample

We used the extra metadata file to pick books in English, and sample 120 books for each of the four categories provided there: prose, poetry, music and drama. We only picked the first volumes for books with more than one volume. Some of the books in the sample did not have an associated fulltext, hence we dropped them, resulting in 452 books/volumes.

More details are given in the [BL_sample notebook](bl_books/BL_sample.ipynb).

## Contracts of apprenticeship in early modern Venice

A set of contracts of apprenticeship from the records of the Archives of Venice. The contracts have been transcribed and then processed into a machine readable spreadsheet.

Download from: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2652855.svg)](https://doi.org/10.5281/zenodo.2652855)

Reference paper: https://www.researchgate.net/publication/318284139_Apprenticeship_in_Early_Modern_Venice.

To read more about this data, see the [project website](https://garzoni.hypotheses.org).

## Early African-American Film Database, 1909–1930

This project was created by UCLA students and faculty members to reconstruct and revive the history of early African-American silent race films.

This dataset contains information on films, actors, production companies, and other aspects of early silent-era African American race films. It is intended to allow the public to learn about this period in film history that is too rarely discussed.

Downloaded from: [![DOI](https://zenodo.org/badge/62099402.svg)](https://zenodo.org/badge/latestdoi/62099402)

Reference paper: https://openhumanitiesdata.metajnl.com/articles/10.5334/johd.7

To read more about this data, see the [project website](http://dhbasecamp.humanities.ucla.edu/afamfilm/).

## Crypto art transactions

A set of transactions of crypto artworks from the [SuperRare gallery](https://superrare.co), roughly from April 2018 to April 2019.

This dataset contains four networks in [GraphML format](http://graphml.graphdrawing.org):
* [Undirected sale network](crypto_art/undirSaleNet.graphml): An undirected network with information about how much total Ether (ETH) was exchanged between two users via sales.
* [Directed sale network](crypto_art/saleNet.graphml): Same as above but directed and with an edge (+ timestamp) for every indivual sale transaction. The graph is thus a multigraph.
* [Directed bid network](crypto_art/bidNet.graphml): Same as above but directed and with an edge (+ timestamp) for every indivual bid transaction. The graph is thus a multigraph. A bid may or may not be accepted and result in a sale.

*Hint: you might want to try Gephi, networkx or igraph to explore this dataset.*

Reference paper: **ADD**

Also see the paper's [original repository](https://github.com/Giovanni1085/art_metrics_public).
