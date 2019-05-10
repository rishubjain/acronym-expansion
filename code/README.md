The codebase is currently divided into jupyter notebooks (I will make some of them scripts, and make them prettier in the next week)

If you are running these scripts, you first need to run these to generate your data and acronyms:

create-acro-dict-playground.ipynb
* creates acros.pickle, which is a dictionary corresponding to all the medical acronyms of wikiepedia (there are some minor annoying parsing issues but arent worth fixing right now)

create_acro_corpus.ipynb
* creates ../brown-data/cleaned_brown_data.csv (which is the list of words in the brown data corpus) and ../brown-data/cleaned_brown_acro_data.csv (which are the random acronyms generated from that corpus)

Then run these to train and test your model:

new-word2vec.ipynb 
* contains the code to train the NCE word2vec model on the medical data (needs to be heavily trimmed and cleaned)
* Classiciation accuracy equivalent to random

new-word2vec-brown.ipynb
* contains the code to train the Softmax word2vec model on the regular text data i.e. the Brown dataset (needs to be slightly cleaned up)
* Got 50% accuracy

new-word2vec-brown-NCEOLDCOPY.ipynb
* contains the code to train the NCE word2vec model on the regular text data i.e. the Brown dataset (needs to be slightly cleaned up)
* Classiciation accuracy equivalent to random



All other notebooks are experimental, and will be deleted from the repo eventually



