# PMI

Postmortem interval (PMI) is the time elapsed since individual's death. When time of death is unknown, PMI is estimated. Forensic scientists can use microbial community composition to estimate PMI. This project is a meta-analysis of PMI studies to address some research gaps in forensic science.

**Goals**

1. What are the difficulties in retrieving data from public databases.
    - Most of the studies we compiled do not publish their scripts
    - Many studies only publish raw sequencing in repositories, and not processed data (e. g., BIOM file)
    - Retrieving large datasets from repositories such as NCBI, EBI, and Qiita, requires knowledge of the command-line and bash scripting, so not really beginner friendly
        - Qiita has functionalities to reanalyze data. But it only works if the studies have raw data publicaly available, have BIOM files publicaly available, and can be easily merged
        - Qiita often has public BIOM files available, but the database is not very straightforward and beginner friendly to retrieve large datasets
        - If working with raw sequencing data, need to double check quality of data. I came across many files in repositories that were empty, aka no sequences, or too short sequences and bad quality

2. What are the difficulties in doing this meta-analysis?
    - Sequencing projects of different amplicon lengths, depths, amplicon region/primer, and sequencing platforms
    - Lack of details about data analysis (e. g., lack of information about parameters and project specific thresholds)
    - Different data analysis software
    - Different databases for taxa assignment
    - Is it possible to combine these heterogeneous studies?
        - merge BIOM files, or start from scratch with raw sequencing data?
