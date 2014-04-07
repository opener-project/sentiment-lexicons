#Sentiment lexicons#

Sentiment lexicons (polarities, aspects) created following several approaches within the OpeNER project.
This is the list of lexicons created and stored in different subfolders:


##lexicons_from_annotations##

Lexicons created from the manual annotated data (which can be found
in also in github, https://github.com/opener-project/opinion_annotations_LANG where $LANG can be
en/es/fr/nl/de/it) using the supervised
heuristic implemented in https://github.com/opener-project/opinion-domain-lexicon-acquisition

##propagation_lexicons##

General lexicons created automatically using the propagation algorithm implemented in https://github.com/opener-project/VU-lexicon-propagation_kernel, and manually
review of the most frequent words for each language. The lexicon comprises the final lexicon after
the manual checking, in CSV and LFM formats, with the manual check items marked explicitly.

These are the parameters used for the automatic propagation of the lexicons:

* Lemma-based output
* Synonymy, antonymy and hyponymy relations of WordNet selected
* Maximum 5 iterations of propagation starting from the seed list (these lists can be found as well in the data)
* Majority voting heuristic for converting synset-based lexicon to lemma-based.



##Contact##
* Ruben Izquierdo
* Vrije University of Amsterdam
* ruben.izquierdobevia@vu.nl
