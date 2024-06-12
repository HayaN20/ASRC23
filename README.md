# ASRC23

Adversarial Search Collection 2023 for "Ranking-Incentivized Document Manipulations for Multiple
Queries" paper.

## Dataset Description

The ASRC23 dataset comprises data from four different competitions:

| Competition | Ranking Function | LLM Tools |
|-------------|------------------|-----------|
| A           | LambdaMART       | ✓         |
| B           | LambdaMART       | ✗         |
| C           | BERT             | ✓         |
| D           | BERT             | ✗         |

Included in the dataset:
- 2520 documents submitted by students, 847 of which are unique.
- 2400 documents generated by bots, 1833 of which are unique.
- 30 initial documents, one per topic.

Documents are stored in "trectext" format.

DOCNO Format: "ROUND-<round_number>-<topic_id>_<competition>-<author_id>"


## Queries

From the UQV dataset, we selected topics with commercial intent likely to stimulate competition. 
Each topic is associated with three queries:
- The **primary query** is the topic (or subtopic) title.
- The **additional two queries** are chosen from a range of query variants related to the topic.

The full list of selected queries is provided in "queries.txt".


## Relevance Judgments

Relevance was assessed by five annotators on Cloudresearch’s Connect platform, based on the topic title and backstory. 
Documents were rated relevant based on their alignment with the stated information need. 
A document’s relevance grade is the count of judges deeming it relevant.

Relevance grades can be found in "documents.rel".


## Quality Judgments

The quality of documents authored by students was also judged by five Cloudresearch annotators. Documents were evaluated as:
1. **Keyword-stuffed** - Contains unnatural repetition of keywords.
2. **Spam** - Content does not meet any conceivable information need.
3. **Valid** - Contents is neither spam nor keyword-stuffed.
A quality grade represents the count of judges who deemed a document valid.

Quality grades can be found in "students_documents.quality".


## Citations

Please cite the ASRC23 dataset as follows when using it in your research:

