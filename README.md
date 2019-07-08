# amharic-word-vectors
fasttext amharic bin loaded to word and vector dicts 
Using the Bert Language Model to put together these vectors means they can be paired with English word vectors in an article from the paire-dnews-corpus, and a language model for Amharic, from those two, can soon have some of the same capabilities as English, despite using tools not at at made for them

Which leads me to a point on the number of words in this list of word vectors; and I'lll just quote Michael Gasser's paper on HornMorpho here. " ..for Semitic languages such as Amharic and Tigri-
nya, morphological analysis can make explicit some of the phonological features of the languages 
that are not reflected in the orthography; these features may be important for text-to-speech applica-
tions. For example, the Tigrinya word ዚፍለጥ ‘which (it) is known’ is correctly pronounced with 
gemination (lengthening) of the third consonant: zifIlleT. The gemination in this case is grammati-
cal, and a morphological analyzer can infer it based on its knowledge of Tigrinya verb roots and the 
particular templates that they occur with.."
This is sigificant for two reasons. One, many approaches to natural language processing that tackle it from a perspective of machine learning often misunderstang the problem at hand, and in this case, it couldn't be more evident. The practice requires data wrangling, language modeling, and semantic concordancing but any sort of CBOW or SKIP gram model or anythign like it is doomed to be ineffective. Two, the exploratory nature of a seq2seq model, for example, harnessed within such a fundamentally different language will yield very very exciting reesults about the practices themselves. The original goal was to contribute to machine translation efforts, or maybe built an enetity recognitizer, but that doesn't seem possible with Semitic languages in the Horn.
