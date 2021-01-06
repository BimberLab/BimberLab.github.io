# Bimber Lab Software

While we are primarily an infectious disease lab, creating software to analyze and manage data is a substantial component of our work. Where possible, we try to package this into broadly useful, stable products and make these available to the broader community. Below are the primary categories of software we generate and support. 


## DISCVR-seq Toolkit

[DISCVR-seq Toolkit](https://bimberlab.github.io/DISCVRSeq/) is a suite of tools written using the GATK4 engine. Many of our sequence and variant analysis tools are writen into this toolkit. These tools include [VariantQC](https://bimberlab.github.io/DISCVRSeq/toolDoc/com_github_discvrseq_walkers_variantqc_VariantQC.html), which can be used to create HTML summary reports from VCF files.  


## LabKey Modules

We heavily use [LabKey Server](https://www.labkey.org) for a range of tasks, including basic lab functions (data and sample management), as well as management and analysis of most of our sequence data.  Our modules fall into several categories:

- [Laboratory Module](https://bimberlab.github.io/DiscvrLabKeyModules/discvr/overview.html): this is the base module for our lab data management and the core of our operations.  It can be used for basic data and experiment management (vaguely like an Electronic Lab Notebook). It is in use beyond our group.

- [SequenceAnalysis](https://bimberlab.github.io/DiscvrLabKeyModules/discvr-seq/overview.html): This module is the core of our sequence data management and analysis. It allows central management of raw data, analysis products, and resources (genomes, gene annotations, etc.).  Related modules allow integration with BLAST, the open source web-based genome browser [JBrowse](https://jbrowse.org/), and our cluster module enables submission of LabKey jobs to either slurm or HTCondor clusters.

- Other notable modules: 
    - OpenLdapSync: This is a standalone module that allows a LabKey Server instance to automatically sync user and/groups with an LDAP Server. LabKey offers a [premium (not free or open source) feature to sync groups](https://www.labkey.org/Documentation/wiki-page.view?name=LDAP_sync). This feature was actually created in 2018 by cloning our code.


## R Packages

- [cellhashR](https://bimberlab.github.io/cellhashR/) is an R package designed to work with cell hashing and CITE-seq data. It can be used for QC of the raw data, as well as generation of cell hashing calls.
- [geneSetViz](https://github.com/BimberLab/geneSetVis) is a R package / Shiny application designed to help interpret set of genes, such as those obtained from RNA-seq experiments. It allows the user to query a given set of genes against many reference sets and pathway tools from a single portal.

## External Contributions

Lab members have contributed to the following projects:

- [GATK3](https://github.com/broadgsa/gatk-protected) and [GATK4](https://github.com/broadinstitute/gatk)
- [Picard Tools](https://github.com/broadinstitute/picard)
- [HTSJDK](https://github.com/samtools/htsjdk)
- [LabKey Server](https://www.labkey.org/home/project-begin.view?)


