# Sarcasm Corpus V2
This page was migrated from https://nlds.soe.ucsc.edu/sarcasm2

**If you use this data in your research, please refer to and cite**: Shereen Oraby, Vrindavan Harrison, Lena Reed, Ernesto Hernandez, Ellen Riloff and Marilyn Walker. ["Creating and Characterizing a Diverse Corpus of Sarcasm in Dialogue."](https://aclanthology.org/W16-3604/) SIGDIAL 2016. Los Angeles, California.

## Overview
The Sarcasm Corpus V2 is a subset of the [Internet Argument Corpus](https://github.com/sl-m-lab/Internet-Argument-Corpus/), including posts annotated for sarcasm. It is an update to the [Sarcasm Corpus V1](https://github.com/slukin/nlds-sarcasm-corpus-v1/tree/main), and contains data representing three categories of sarcasm: general sarcasm, hyperbole, and rhetorical questions.

## Data
This updated download now contains the full Sarcasm Corpus V2 from the paper. ~~This download is currently a random sample of the dataset - the full corpus will be released as we continue to add more data.~~

The largest subset of the sample is the generic sarcasm subset (GEN), containing 3,260 posts per class (sarcastic and not-sarcastic, for a total of 6,520 posts). The HYP and RQ samples are smaller, containing 582 and 851 posts per class, respectively. Some of the posts in the HYP and RQ samples are instances also existing in the GEN corpus, exhibiting sarcastic/not-sarcastic instances of hyperbole or rhetorical questions. HYP posts contain cue words signaling hyperbole, and RQ posts contain question-answer pairs where the speaker continues with their turn (not allowing a direct answer to their question).

The sample is a single CSV file with the following fields:

- Corpus: The corpus type - one of GEN (general sarcasm), HYP (hyperbole), and RQ (rhetorical questions).
- Label: The class label of the response utterance - one of "sarc" (sarcastic) or "notsarc" (not-sarcastic)
- ID: A unique ID for the post. Pairs with the same ID numbers across different datasets are not related.
- Text: The text of the post, annotated for sarcasm (i.e. the sarcasm label relates to this utterance).