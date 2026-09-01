# Brodsky in Italian: A TEI/XML Edition of *Poesie Italiane*

Italy became a third homeland for the Russian and American poet Joseph Brodsky, and it holds an important place in his work. Many of his texts have been translated into Italian, but there is no organized digital archive of Brodsky in Italian. This repository presents a TEI/XML encoding of *Poesie Italiane* (the original with a parallel Italian translation) with NER tagging, which can form part of such an archive and be used in philological studies of Brodsky's poetry.

## Contents

| File | Description |
|------|-------------|
| `brodsky_final_15-10-2025.xml` | Main file: the full TEI/XML encoding |
| `Brodsky_tags&attributes.pdf` | Detailed commentary on every tag and attribute used in the encoding |
| `*.csv` | Datasets of places and persons used for NER tagging, and data on the preservation of rhyme in translation |
| `tagging_loc_and_pers.ipynb` | Automatic tagging of places and persons, and aggregation of `listPlace` and `listPerson` |
| `tags_and_attributes.ipynb` | Prints the full list of tags and attributes used in the encoding |

## Notes on the encoding

Minor changes were made to both the datasets and the notebook output after the code was run, in order to match the TEI guidelines. For example, the `city` tag was replaced by `settlement type="city"`, and the `type` and `role` tags for persons by the `trait` tag.

## Additional materials

A nicer dataset preview and a map presentation of the coordinates are available [here](https://drive.google.com/drive/folders/1zGWD7sMZ61VjUgyJD6VzmBRr488NabrC?usp=sharing).

## License

This repository contains both code and data, which are licensed separately:

- **Code** (`tags_and_attributes.ipynb`, `tagging_loc_and_pers.ipynb`) — MIT License, see [`LICENSE`](LICENSE).
- **TEI encoding, annotation, and derived datasets** (`brodsky_final_15-10-2025.xml`, `.csv` files) — CC BY 4.0, see [`LICENSE-DATA`](LICENSE-DATA).

The underlying poems by Joseph Brodsky and their Italian translations remain under their respective copyrights and are reproduced here for scholarly and educational purposes only.
