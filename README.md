# MIRACL 🌍🙌🌏

## Overview

MIRACL 🌍🙌🌏 (Multilingual Information Retrieval Across a Continuum of Languages) is an WSDM 2023 Cup challenge that focuses on search across 18 different languages, which collectively encompass over three billion native speakers around the world.
The website for the event can be found at [`miracl.ai`](http://miracl.ai).
The repo provides pointers to accessing the actual dataset.

If you're interested in hearing updates, please join our [mailing list](https://forms.gle/aCbjRQ9CPeXViWcaA).

## Corpus

The corpus is available as a [HuggingFace Dataset](https://huggingface.co/datasets/miracl/miracl-corpus).
So far, we have released data for the 16 "known languages".
There remain 2 "surprise languages" that will not be released until later.
See our release schedule [on the MIRACL website](http://miracl.ai).

The corpus are prepared from Wikipedia dumps, where we keep only the plain text information and disgard the image, table, etc.
Each article is segmented into multiple passages via [WikiExtractor](https://github.com/attardi/wikiextractor) based on natural discourse units (e.g., `\n\n` in the wiki markup).
We preserve the Wikipedia article title to each passage.

Our collection data files are in `jsonlines`, compressed with `gzip`. Each line in the file corresponding to a passage, in the format of `{"docid": ..., "title": ..., "text": ...}`. An example from English collection:

```
{
    "docid": "39#0",
    "title": Albedo, 
    "text": "Albedo (meaning 'whiteness') is the measure of the diffuse reflection of solar radiation out of the total solar radiation received by an astronomical body (e.g. a planet like Earth). It is dimensionless and measured on a scale from 0 (corresponding to a black body that absorbs all incident radiation) to 1 (corresponding to a body that reflects all incident radiation)."
}
```

The statistics of MIRACL corpus:
| Language        | # of Passage | # of Docs |
|:----------------|-------------:|----------:|
| Arabic (ar)     |    2,061,414 |   656,982 |
| Bengali (bn)    |      297,265 |    63,762 |
| English (en)    |   32,893,221 | 5,758,285 |
| Spanish (es)    |   10,373,953 | 1,669,181 |
| Persian (fa)    |    2,207,172 |   857,827 |
| Finnish (fi)    |    1,883,509 |   447,815 |
| French (fr)     |   14,636,953 | 2,325,608 |
| Hindi (hi)      |      506,264 |   148,107 |
| Indonesian (id) |    1,446,315 |   446,330 |
| Japanese (ja)   |    6,953,614 | 1,133,444 |
| Korean (ko)     |    1,486,752 |   437,373 |
| Russian (ru)    |    9,543,918 | 1,476,045 |
| Swahili (sw)    |      131,924 |    47,793 |
| Telugu (te)     |      518,079 |    66,353 |
| Thai (th)       |      542,166 |   128,179 |
| Chinese (zh)    |    4,934,368 | 1,246,389 |


## Relevance Judgments

Coming soon!
See our release schedule [on the MIRACL website](http://miracl.ai).

## Contact

If you have any questions, feel free to email us (project.miracl [at] gmail.com) or start a Github issue under this repository. 
