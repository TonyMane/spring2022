Basic manipulations of phyloseq objects. Rarefying sample species tables (or sample approximate sequence variant/operational taxonomic unit tables),
subsetting sample data (by time or data type), calculating distance metrics, phylogenetic analyses, ordinations. Does not include the creation of phyloseq
object or incorporation of meta-data (see https://github.com/TonyMane/caddis/blob/main/tutorial_dada2_to_phyloseq.md). For background on phyloseq  see
https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0061217 or https://joey711.github.io/phyloseq/). 

```
library(phyloseq)
library(ape)
load("caddis03282022.rds")
```
The rds file should be very simple, containing a sinlge object. 
Can just type 'objects()' do see see whats been loaded.

```
objects()
[1] "ps"
```
Some basic data about the object can be printed by typing its name.

```
ps
phyloseq-class experiment-level object
otu_table()   OTU Table:         [ 69382 taxa and 219 samples ]
sample_data() Sample Data:       [ 219 samples by 4 sample variables ]
tax_table()   Taxonomy Table:    [ 69382 taxa by 6 taxonomic ranks ]
refseq()      DNAStringSet:      [ 69382 reference sequences ]
```
