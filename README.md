#Sentiment lexicons#

This repository contains the lexicons created automatically from the OpeNER hotel annotations and by applying a technique to find
words related with hotel ratings.

##lexicons_from_annotations##
Lexicons created from the manual annotated data (this data can
 be found also in github, https://github.com/opener-project/opinion_annotations_LANG where
 $LANG can be en/es/fr/nl/de/it) using the supervised 
heuristic implemented in https://github.com/opener-project/opinion-domain-lexicon-acquisition

##rating_lexicons##

This folder contains lexicons for 1-, 2- and 3-grams of expressions associated with star ratings. They have been compiled automatically for
English and Dutch using our domain acquisition toolkit (https://github.com/opener-project/opinion-domain-lexicon-acquisition) and a large
set of hotel reviews for these 2 languages. All these reviews have been crawled automatically and the star rating is available. This rating
ranges from 0 to 100, and we have normalised it to a range 1-5. The 1-star reviews have been merged with the 2-starts reviews as there
were just few reviews labeled with 1-star. The format of these lexicons is CSV, one file per ngram type, so for instance in the tri-gram English
file we can find this line:
```shell
definitely be returning;5;2.02;5=-10.9 4=-14.94
```

The first field is the actual word or ngram, the second field is the star rating
more strongly associated with this word and the third is the standard deviation of the
values of association of the words with each rating (the lexicon is sorted according
to this value). The last field are the values of association of the ngram with each
star rating.

##Contact##
* Ruben Izquierdo
* Vrije University of Amsterdam
* ruben.izquierdobevia@vu.nl
