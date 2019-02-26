# Bimber Lab Software

While we are primarily an infectious disease lab, creating software to analyze and manage data is a substantial component of our work. Where possible, we try to package this into broadly useful, stable products and make these available to the broader community. Below are the primary categories of software we generate and support. 


## DISCVR-seq Toolkit

[DISCVR-seq Toolkit](https://bimberlab.github.io/DISCVRSeq/) is a suite of tools written using the GATK4 engine. Many of our sequence and variant analysis tools are writen into this toolkit. These tools include [VariantQC](https://bimberlab.github.io/DISCVRSeq/toolDoc/com_github_discvrseq_walkers_variantqc_VariantQC.html), which can be used to create HTML summary reports from VCF files.  


## LabKey Modules

We heavily use [LabKey Server](https://www.labkey.org) for a range of tasks, including basic lab data and sample management (Laboratory module), management and analysis of sequence data (SequenceAnalysis module), and more:

- Laboratory: this is the base module for our lab data management.  It can be used for basic data and experiment management (vaguely like an Electronic Lab Notebook).

- SequenceAnalysis: This module is the core of how we manage sequence data. It allows central management of raw data, analysis products, and resources (genomes, gene annotations, etc.). 

  - Blast: This allows users to create custom BLAST databases and submit BLAST searches through LabKey. 

  - JBrowse: This module bundles [JBrowse](https://jbrowse.org/), an open source web-based genome browser, to allow users to create custom genome browser sessions to view data managed in LabKey.

- Cluster: This module allows LabKey pipeline jobs to be submitted to HTCondor or Slurm clusters. 

- OmeroIntegration: This is a functional, although primarily proof-of-concept, module to demonstrate how LabKey Server can interact with Omero, an open-source platform to manage images. If the LabKey Server stores the IDs of images in Omero, it can render thumbnails in a LabKey grid, and open the Omero image viewer inline to inspect these images.

- OpenLdapSync: This is a standalone module that allows a LabKey Server instance to automatically sync user and/groups with an LDAP Server. LabKey offer a premium (not free or open source) feature to sync groups. This feature was actually created in 2018 by cloning our code.


## R Packages

Coming Soon.
