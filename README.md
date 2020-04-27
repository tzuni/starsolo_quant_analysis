# Analysis of StarSolo smartseq quantification at Gene and GeneFull levels

Star Solo aligns and quantifies single cell RNA seq data in a convenient single command. It works with 10x and SmartSeq style data (though the latter is in a development branch only at time of writing). I noticed an unexpected result where quantification at the `GeneFull` level which includes intron reads resulted in generally lower read counts than in the `Gene` mode which only counts reads aligned to exons.

This is an exploration of that oddity and how gene feature overlap affects quantification. There are two notebooks, one can be used to determine overlap and coverage per gene feature in a given GTF file, the other has the 

- determine overlap and coverage per gene feature in GTF : [notebooks/get_gtf_info.ipynb](notebooks/get_gtf_info.ipynb)
- how overlap affects quantification in an scRNA smartseq data set : [notebooks/star_solo_gene_genefull_plot.ipynb](notebooks/star_solo_gene_genefull_plot.ipynb)

