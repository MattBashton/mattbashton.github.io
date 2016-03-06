---
layout: post
title: Contributing to the OpenAshDieBack crowd sourced effort
comments: true
excerpt_separator: <!--more-->
---

_Originally posted on 12th of February 2013_

Just before finishing for Christmas last year I became interested in the [crowd sourced effort](http://oadb.tsl.ac.uk/) to analyse the fungal disease currently affecting ash trees.  The disease is caused by the [_Hymenoscyphus fraxineus_](https://en.wikipedia.org/wiki/Hymenoscyphus_fraxineus) fungus. The data for the project was quickly released following initial sequencing runs via [GitHub](https://github.com/). This is similar to an approach taken with sequencing data from the [german E. coli O104:H4 outbreak](https://github.com/ehec-outbreak-crowdsourced/BGI-data-analysis) and meant various scientists around the world could get their hands on the raw data and contribute analysis of it to the collective effort by uploading their results directly to GitHub.
<!--more-->

So far I have contributed:

- [FastQC](https://github.com/ash-dieback-crowdsource/data/tree/master/ash_dieback/mixed_material/FastQC) reports of the released RNAseq reads.

- Assemblies of both the [AT1](https://github.com/ash-dieback-crowdsource/data/tree/master/ash_dieback/mixed_material/ashwellthorpe_AT1/assemblies) and [AT2](https://github.com/ash-dieback-crowdsource/data/tree/master/ash_dieback/mixed_material/ashwellthorpe_AT2/assemblies) mixed interaction transcriptome produced using [Trinity](https://github.com/trinityrnaseq/trinityrnaseq/wiki), this contained reads from both the fungus and host tree, although most of the material appeared to be fungal.

- Likely coding sequences for both the Trinity derived [AT1](https://github.com/ash-dieback-crowdsource/data/tree/master/ash_dieback/mixed_material/ashwellthorpe_AT1/likely_coding_sequences) and [AT2](https://github.com/ash-dieback-crowdsource/data/tree/master/ash_dieback/mixed_material/ashwellthorpe_AT2/likely_coding_sequences) transcripts.

- [Pfam](http://pfam.xfam.org/) and [SUPERFAMILY](http://supfam.org/SUPERFAMILY/) HMM based domain assignments for these coding sequences, [here](https://github.com/ash-dieback-crowdsource/data/tree/master/ash_dieback/mixed_material/ashwellthorpe_AT1/PfamA_Vs_AT1_CDS), [here](https://github.com/ash-dieback-crowdsource/data/tree/master/ash_dieback/mixed_material/ashwellthorpe_AT1/SUPERFAMILY_domain_assignments), [here](https://github.com/ash-dieback-crowdsource/data/tree/master/ash_dieback/mixed_material/ashwellthorpe_AT2/PfamA_Vs_AT2_CDS) and [here](https://github.com/ash-dieback-crowdsource/data/tree/master/ash_dieback/mixed_material/ashwellthorpe_AT2/SUPERFAMILY_domain_assignments).

- Detected [NPP1-like necrosis inducing protein domains](http://www.sciencedirect.com/science/article/pii/S0031942205006758) (aka Nep1-like proteins) found in the [AT1](https://github.com/ash-dieback-crowdsource/data/tree/master/ash_dieback/mixed_material/ashwellthorpe_AT1/NPP1_domains) and [AT2](https://github.com/ash-dieback-crowdsource/data/tree/master/ash_dieback/mixed_material/ashwellthorpe_AT2/NPP1_domains) samples using the HMM for the [NPP1 Pfam family](http://pfam.xfam.org/family/PF05630) with [HMMER](http://hmmer.org/).

- A [multiple alignment](https://github.com/ash-dieback-crowdsource/data/tree/master/ash_dieback/mixed_material/Helotiales_NPP1_domains_and_AT1_AT2_NPP1_aligned) of all AT1 and AT2 NPP1-like necrosis inducing proteins domains aligned with fungal homologues from the [Helotiales](https://en.wikipedia.org/wiki/Helotiales) order (which contains many plant pathogens) detected using an iterative [Jackhmmer](https://www.ebi.ac.uk/Tools/hmmer/search/jackhmmer) run (using the AT1 and AT2 sequences as a seed) over Uniprot.  _Hymenoscyphus fraxineus_ is its self part of this order so considering other necrosis inducing proteins from similar pathogenic fungi my be useful for investigating pathogenesis.

An initial publication detailing the crowd sourced effort has been published in [GigaScience](http://gigascience.biomedcentral.com/articles/10.1186/2047-217X-2-2).  Currently I’m quite busy with a number of projects here at Newcastle but I hope to contribute more analysis to this project soon.
