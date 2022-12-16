# DanteLatinLoanWords
# Resource description

The Glossary of Latin loanwords from the Italian works of Dante Alighieri was developed by Giulia Pedonese during her PhD course in Italian linguistics and collects 765 Italian words which are Latin loanwords attested in the four Italian works by XIIIth Century writer and poet Dante Alighieri.

The texts of these works (Rime, Vita Nova, Convivio and Commedia) are taken from the same reference editions that form the basis of DanteSearch (https://dantesearch.dantenetwork.it/), a digital corpus collecting Dante's Italian and Latin works lemmatised with grammatical and syntactic marking.

# Current status
At present, each one of the 756 lemmas of the resource was linked to the LiLa Lemma Bank (https://github.com/CIRCSE/LiLa_Lemma-Bank) through the corresponding Latin lemma from which the loan was taken.

The glossary also includes information relevant to the historical linguistic framing of the loan, such as the loan type and its relative position of first attestation or hapax legomenon in the lexicon of XIIIth Century Italian. 

In the next future, these data will be modeled using custom ontologies.

# Linking process

Each Latin word corresponding to the loanword has been matched with one or more lemmas in the Lemma Bank. Of the total of 765 lemmas:

- 740 lemmas were automatically matched with a 1:1 ratio. 

- 20 lemmas had a 1:0 match in the Lemma Bank. In those cases, we proceeded to manually add 15 new lemmas, 2 new written representations and 3 new lemma variants to the Lemma Bank.

- 5 lemmas had a one-to-many match. In 4 cases, it was false ambiguity since the link was made to several lemmas connected to each other by the relationship 'lemma variant'. Only 1 lemma was left ambiguous since the etymology of the Latin loanword in ancient Italian is still discussed.


# Modeling

1. Each loanword is modeled as a Form linked to its Lexical Entry via the property canonicalForm according the Ontolex-Lemon ontology.
2. The Latin etymology is expressed as the Etymon class in LemonEty (the Ontolex-Lemon Etymological Extension) which is a subclass of Ontolex's Lexical Entry.
3. The Italian Lexical Entry and its Latin Etymon are linked through the class Etymology, which allows to represent etymologies as a set of propositions about the history of the word, possibly adding information such as the attribution to scholars and bibliographical references.
4. Attached to the Etymology is the class Etymology Link that could be used in the future to further specify the link between the Lexical Entry of the loanword and its Etymon by defining the type of relations they imply (e.g. the type of borrowing, which in this case may be phono-morphological, semantic or due to translation), see section 'Current status' above.

# Credits

Creator: Giulia Pedonese
Contributors: Marco Passarotti, Francesco Mambrini, Giovanni Moretti

The LiLa: Linking Latin project has received funding from the European Research Council (ERC) under the European Union's Horizon 2020 research and innovation programme – Grant Agreement No. 769994.

# Copyright

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.

# Citation

Zenodo link
