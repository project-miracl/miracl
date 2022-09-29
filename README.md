# MIRACL 🌍🙌🌏

## Overview

MIRACL 🌍🙌🌏 (Multilingual Information Retrieval Across a Continuum of Languages) is an WSDM 2023 Cup challenge that focuses on search across 18 different languages, which collectively encompass over three billion native speakers around the world.
The website for the event can be found at [`miracl.ai`](http://miracl.ai).
This repo provides pointers to accessing the actual dataset.

If you're interested in hearing updates, please join our [mailing list](https://forms.gle/aCbjRQ9CPeXViWcaA).

## Corpora

The corpora used in MIRACL is available as a [HuggingFace Dataset](https://huggingface.co/datasets/miracl/miracl-corpus).
So far, we have released data for the 16 "known languages".
The remaining 2 "surprise languages" will not be released until later.
See our release schedule [on the MIRACL website](http://miracl.ai).

The corpus for each language is prepared from a Wikipedia dump, where we keep only the plain text and discard images, tables, etc.
Each article is segmented into multiple passages using [WikiExtractor](https://github.com/attardi/wikiextractor) based on natural discourse units (e.g., `\n\n` in the wiki markup).
Each of these passages comprise a "document" or unit of retrieval.
We preserve the Wikipedia article title of each passage.

The corpus data files are in [JSON lines](https://jsonlines.org/) format, compressed with `gzip`.
Each line in the file corresponds to a passage.
Consider an example from the English corpus:

```
{
    "docid": "39#0",
    "title": "Albedo", 
    "text": "Albedo (meaning 'whiteness') is the measure of the diffuse reflection of solar radiation out of the total solar radiation received by an astronomical body (e.g. a planet like Earth). It is dimensionless and measured on a scale from 0 (corresponding to a black body that absorbs all incident radiation) to 1 (corresponding to a body that reflects all incident radiation)."
}
```

The `docid` has the schema `X#Y`, where all passages with the same `X` come from the same Wikipedia article, whereas `Y` denotes the passage within that article, numbered sequentially.
The `text` field contains the text of the passage.
The `title` field contains the name of the article the passage comes from.

Statistics of the MIRACL corpora:

| Language        | # of Passage | # of Docs | Links |
|:----------------|-------------:|----------:|:------|
| Arabic (ar)     |    2,061,414 |   656,982 | [[Direct Link](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-ar)] |
| Bengali (bn)    |      297,265 |    63,762 | [[Direct Link](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-bn)] |
| English (en)    |   32,893,221 | 5,758,285 | [[Direct Link](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-en)] |
| Spanish (es)    |   10,373,953 | 1,669,181 | [[Direct Link](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-es)] |
| Persian (fa)    |    2,207,172 |   857,827 | [[Direct Link](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-fa)] |
| Finnish (fi)    |    1,883,509 |   447,815 | [[Direct Link](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-fi)] |
| French (fr)     |   14,636,953 | 2,325,608 | [[Direct Link](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-fr)] |
| Hindi (hi)      |      506,264 |   148,107 | [[Direct Link](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-hi)] |
| Indonesian (id) |    1,446,315 |   446,330 | [[Direct Link](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-id)] |
| Japanese (ja)   |    6,953,614 | 1,133,444 | [[Direct Link](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-ja)] |
| Korean (ko)     |    1,486,752 |   437,373 | [[Direct Link](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-ko)] |
| Russian (ru)    |    9,543,918 | 1,476,045 | [[Direct Link](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-ru)] |
| Swahili (sw)    |      131,924 |    47,793 | [[Direct Link](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-sw)] |
| Telugu (te)     |      518,079 |    66,353 | [[Direct Link](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-te)] |
| Thai (th)       |      542,166 |   128,179 | [[Direct Link](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-th)] |
| Chinese (zh)    |    4,934,368 | 1,246,389 | [[Direct Link](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-zh)] |


## Relevance Judgments

Coming soon!
See our release schedule [on the MIRACL website](http://miracl.ai).

## Contact

If you have any questions, feel free to email us (project.miracl [at] gmail.com) or start a Github issue under this repository. 
