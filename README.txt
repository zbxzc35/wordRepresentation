Author: Devan Hawkins
Date: March 19, 2015

Note: Numpy libraries are needed to run these files.

Run Instructions are given in terms of iPython. Type these intrsuctions in verbatim.

1) ipython

2) import cPickle, language_model

3) data = cPickle.load(open(’data.pk’, ’rb’))

4) model = language_model.train(16, 128)
   *Note: This will take a few minutes.*
(optional) model.tsne_plot()
           OR you can open "snapshot1.png" to see the spatial representation.

From here, you can chose are three words that exist in the vocabulary (see raw_sentences.txt) and use "model.predict_next_word('word1','word2','word3')" to have the network make a few guesses.

For example, 
model.predict_next_word('what','time','is') 
model.predict_next_word('life','in','the') 
model.predict_next_word('i','want','to') 
model.predict_next_word('where','is','my') 