<!-- <p align="center"> <span><font size="32"> <b> MIRACL 🌍🙌🌏 </b></font></span></p> -->
<h1 align="center"> 
    <img style="vertical-align:middle" width="2000" alt="image" src="https://user-images.githubusercontent.com/31640436/210273474-7697ab15-c638-4513-8c80-12886941f520.png">
</h1>

<p align="center">
    <a href="https://www.python.org/">
            <img alt="Build" src="https://img.shields.io/badge/Made%20with-Python-1f425f.svg?color=purple">
    </a>
    <a href="https://github.com/beir-cellar/beir/blob/master/LICENSE">
        <img alt="License" src="https://img.shields.io/github/license/beir-cellar/beir.svg?color=green">
    </a>
    <a href="https://github.com/beir-cellar/beir/">
        <img alt="Downloads" src="https://badges.frapsoft.com/os/v1/open-source.svg?v=103">
    </a>
</p>

<h4 align="center">
    <p>
        <a href="https://arxiv.org/abs/2210.09984">Paper</a> |
        <a href="#-baselines">Baselines</a> |
        <a href="https://huggingface.co/datasets/miracl">HuggingFace</a> |
        <a href="https://eval.ai/web/challenges/challenge-page/1881/leaderboard">Leaderboard</a>
    </p>
</h4>



## 🙌 MIRACL

MIRACL 🌍🙌🌏 (Multilingual Information Retrieval Across a Continuum of Languages) is an WSDM 2023 Cup challenge that focuses on search across 18 different languages, which collectively encompass over three billion native speakers around the world.
The website for the event can be found at [`miracl.ai`](http://miracl.ai).
This repo provides pointers to access the actual dataset.

For more details, check out our arXiv paper: [Making a MIRACL: Multilingual Information Retrieval Across a Continuum of Languages](https://arxiv.org/abs/2210.09984).

Connect with us!
- 📬 [Mailing list](https://forms.gle/aCbjRQ9CPeXViWcaA)
- 💬 [Slack Workspace](https://join.slack.com/t/miraclgroup/shared_invite/zt-1ph43qw40-gvoQI~jc_g2EPb_EgCF4Dg)
- 📣 [Twitter](https://twitter.com/project_miracl?s=21&t=Qf9LrVerhhN1hsXs1gdWhw)

## 🙌 Corpora

The Wikipedia corpora used in MIRACL are available as a [HuggingFace Dataset](https://huggingface.co/datasets/miracl/miracl-corpus).
So far, we have released corpora for the 16 "known languages"; the remaining 2 "surprise languages" will be revealed later!

+ 🤗 = direct link to HuggingFace Dataset
+ 🌏 = link to raw wiki dumps

| Language        | # of Passages | # of Articles | Links |
|:----------------|--------------:|--------------:|:------|
| Arabic (ar)     |     2,061,414 |       656,982 | [🤗](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-ar) [🌏](https://archive.org/download/arwiki-20190201/arwiki-20190201-pages-articles-multistream.xml.bz2)
| Bengali (bn)    |       297,265 |        63,762 | [🤗](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-bn) [🌏](https://archive.org/download/bnwiki-20190201/bnwiki-20190201-pages-articles-multistream.xml.bz2)
| English (en)    |    32,893,221 |     5,758,285 | [🤗](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-en) [🌏](https://archive.org/download/enwiki-20190201/enwiki-20190201-pages-articles-multistream.xml.bz2)
| Spanish (es)    |    10,373,953 |     1,669,181 | [🤗](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-es) [🌏](https://archive.org/download/eswiki-20220301/eswiki-20220301-pages-articles-multistream.xml.bz2)
| Persian (fa)    |     2,207,172 |       857,827 | [🤗](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-fa) [🌏](https://archive.org/download/fawiki-20220301/fawiki-20220301-pages-articles-multistream.xml.bz2)
| Finnish (fi)    |     1,883,509 |       447,815 | [🤗](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-fi) [🌏](https://archive.org/download/fiwiki-20190201/fiwiki-20190201-pages-articles-multistream.xml.bz2)
| French (fr)     |    14,636,953 |     2,325,608 | [🤗](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-fr) [🌏](https://archive.org/download/frwiki-20220301/frwiki-20220301-pages-articles-multistream.xml.bz2)
| Hindi (hi)      |       506,264 |       148,107 | [🤗](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-hi) [🌏](https://archive.org/download/hiwiki-20220301/hiwiki-20220301-pages-articles-multistream.xml.bz2)
| Indonesian (id) |     1,446,315 |       446,330 | [🤗](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-id) [🌏](https://archive.org/download/idwiki-20190201/idwiki-20190201-pages-articles-multistream.xml.bz2)
| Japanese (ja)   |     6,953,614 |     1,133,444 | [🤗](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-ja) [🌏](https://archive.org/download/jawiki-20190201/jawiki-20190201-pages-articles-multistream.xml.bz2)
| Korean (ko)     |     1,486,752 |       437,373 | [🤗](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-ko) [🌏](https://archive.org/download/kowiki-20190201/kowiki-20190201-pages-articles-multistream.xml.bz2)
| Russian (ru)    |     9,543,918 |     1,476,045 | [🤗](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-ru) [🌏](https://archive.org/download/ruwiki-20190201/ruwiki-20190201-pages-articles-multistream.xml.bz2)
| Swahili (sw)    |       131,924 |        47,793 | [🤗](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-sw) [🌏](https://archive.org/download/swwiki-20190201/swwiki-20190201-pages-articles-multistream.xml.bz2)
| Telugu (te)     |       518,079 |        66,353 | [🤗](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-te) [🌏](https://archive.org/download/tewiki-20190201/tewiki-20190201-pages-articles-multistream.xml.bz2)
| Thai (th)       |       542,166 |       128,179 | [🤗](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-th) [🌏](https://archive.org/download/thwiki-20190101/thwiki-20190101-pages-articles-multistream.xml.bz2)
| Chinese (zh)    |     4,934,368 |     1,246,389 | [🤗](https://huggingface.co/datasets/miracl/miracl-corpus/tree/main/miracl-corpus-v1.0-zh) [🌏](https://archive.org/download/zhwiki-20220301/zhwiki-20220301-pages-articles-multistream.xml.bz2)

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

## 🙌 Topics and Relevance Judgments

Topics (= queries) and relevance judgments (= relevance labels) of the MIRACL training sets and development sets for each of the 16 known languages are  available on [HuggingFace Dataset](https://huggingface.co/datasets/miracl/miracl)! 

🤗 = direct link to HuggingFace Dataset

|  | Train |        |  Dev  |        |  |
|:-----|------:|-------:|------:|-------:|:-----|
| **Language**     | **#Q**| **#J** |**#Q** |**#J**  | **Links** |
| Arabic (ar)     | 3,495 | 25,382 | 2,896 | 29,197 | [🤗](https://huggingface.co/datasets/miracl/miracl/tree/main/miracl-v1.0-ar) |
| Bengali (bn)    | 1,631 | 16,754 |   411 |  4,206 | [🤗](https://huggingface.co/datasets/miracl/miracl/tree/main/miracl-v1.0-bn) |
| English (en)    | 2,863 | 29,416 |   799 |  8,350 | [🤗](https://huggingface.co/datasets/miracl/miracl/tree/main/miracl-v1.0-en) |
| Spanish (es)    | 2,162 | 21,531 |   648 |  6,443 | [🤗](https://huggingface.co/datasets/miracl/miracl/tree/main/miracl-v1.0-es) |
| Persian (fa)    | 2,107 | 21,844 |   632 |  6,571 | [🤗](https://huggingface.co/datasets/miracl/miracl/tree/main/miracl-v1.0-fa) |
| Finnish (fi)    | 2,897 | 20,350 | 1,271 | 12,008 | [🤗](https://huggingface.co/datasets/miracl/miracl/tree/main/miracl-v1.0-fi) |
| French (fr)     | 1,143 | 11,426 |   343 |  3,429 | [🤗](https://huggingface.co/datasets/miracl/miracl/tree/main/miracl-v1.0-fr) |
| Hindi (hi)      | 1,169 | 11,668 |   350 |  3,494 | [🤗](https://huggingface.co/datasets/miracl/miracl/tree/main/miracl-v1.0-hi) |
| Indonesian (id) | 4,071 | 41,358 |   960 |  9,668 | [🤗](https://huggingface.co/datasets/miracl/miracl/tree/main/miracl-v1.0-id) |
| Japanese (ja)   | 3,477 | 34,387 |   860 |  8,354 | [🤗](https://huggingface.co/datasets/miracl/miracl/tree/main/miracl-v1.0-ja) |
| Korean (ko)     |   868 | 12,767 |   213 |  3,057 | [🤗](https://huggingface.co/datasets/miracl/miracl/tree/main/miracl-v1.0-ko) |
| Russian (ru)    | 4,683 | 33,921 | 1,252 | 13,100 | [🤗](https://huggingface.co/datasets/miracl/miracl/tree/main/miracl-v1.0-ru) |
| Swahili (sw)    | 1,901 |  9,359 |   482 |  5,092 | [🤗](https://huggingface.co/datasets/miracl/miracl/tree/main/miracl-v1.0-sw) |
| Telugu (te)     | 3,452 | 18,608 |   828 |  1,606 | [🤗](https://huggingface.co/datasets/miracl/miracl/tree/main/miracl-v1.0-te) |
| Thai (th)       | 2,972 | 21,293 |   733 |  7,573 | [🤗](https://huggingface.co/datasets/miracl/miracl/tree/main/miracl-v1.0-th) |
| Chinese (zh)    | 1,312 | 13,113 |   393 |  3,928 | [🤗](https://huggingface.co/datasets/miracl/miracl/tree/main/miracl-v1.0-zh) |
| **Total**       | 40,203 | 343,177 | 13,071 | 126,076 |

The above table shows the number of queries (`#Q`) and the number of judgments (`#J`) in each (language, split) combination, where the judgments include both positive and negative labels.

The topics are formatted in TSV, with each line organized as follows:

```
qid\tquery
```

The relevance judgments are formatted in standard TREC qrels format, as follows:

```
qid Q0 docid relevance
```

## 🙌 Baselines

We have released baselines using BM25, mDPR, and hybrid of the two, as described in our [arXiv paper](https://arxiv.org/abs/2210.09984). 
Reuslts of BM25 and mDPR could be reproduced using [Pyserini](https://github.com/castorini/pyserini).

To reproduce our baselines:

1. Install the development version of Pyserini following [these instructions](https://github.com/castorini/pyserini/blob/master/docs/installation.md#development-installation). **(To run baselines on surprise languages, you'll need to re-build both Anserini and Pyserini)**
2. Manually place all topics and qrels files under `tools/topics-and-qrels`. The topics and qrels files can be found under `miracl-v1.0-${lang}/topics` and `miracl-v1.0-${lang}/qrels` in the [HuggingFace dataset](https://huggingface.co/datasets/miracl/miracl). 
    ```
    git clone https://huggingface.co/datasets/miracl/miracl
    mv miracl/*/*/* $PYSERINI_PATH/tools/topics-and-qrels/
    ```
3. Following the commands in our [2-click-reproduction (2CR) website](https://castorini.github.io/pyserini/2cr/miracl.html).

## 🙌 Citation
If you find this dataset and repository helpful, please cite MIRACL as follows:
```
@article{miracl,
      title={Making a {MIRACL}: Multilingual Information Retrieval Across a Continuum of Languages}, 
      author={Xinyu Zhang and Nandan Thakur and Odunayo Ogundepo and Ehsan Kamalloo and David Alfonso-Hermelo and Xiaoguang Li and Qun Liu and Mehdi Rezagholizadeh and Jimmy Lin},
      year={2022},
      journal={arXiv:2210.09984},
}
```

## 🙌 Contact

If you have any questions, feel free to email us (project.miracl [at] gmail.com) or start a Github issue under this repository. 
