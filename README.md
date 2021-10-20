# Lab kraken2

**[ Kraken 2](https://github.com/DerrickWood/kraken2/wiki/About-Kraken-2)** is one of the most popular tools used for assigning taxonomic labels to short DNA sequences.  

At the core of [Kraken](https://genomebiology.biomedcentral.com/articles/10.1186/gb-2014-15-3-r46) is a database that contains records consisting of a k-mer and the LCA of all organisms whose genomes contain that k-mer. This database, built using a user-specified library of genomes, allows a quick lookup of the most specific node in the taxonomic tree that is associated with a given k-mer. Sequences are classified by querying the database for each k-mer in a sequence, and then using the resulting set of LCA taxa to determine an appropriate label for the sequence. Sequences that have no k-mers in the database are left unclassified by Kraken. 
