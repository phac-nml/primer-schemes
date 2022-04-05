# primer-schemes
Schemes for SarsCoV2 sequencing to be used in sequence analysis pipelines

## Files

| File | Info |
|-|-|
| .primer.bed; .bed; .scheme.bed | Different formats for the coordinates of each primer in the scheme |
| .reference.fasta | Reference fasta genome |
| ncov-qc_*.scheme.bed | Sequencing amplicons for ncov-tools |

### File Format Clarifications 2022-04-05
- `<NAME>.bed` coordinates file used by ncov-tools
- `<NAME>.scheme.bed` coordinates file used by ARTIC fieldbioinformatics minion pipeline
    - Had to add the "nCoV-2019" versions for `V4` and `V4.1` to match other schemes for the pipeline
        - Could have linked the "nCoV-2019" directory as "SARS-CoV-2" instead but adding the files for the moment is a bit cleaner
- `ncov-qc_*.scheme.bed` amplicon coordinates with the "nCoV-2019" naming convention

## Schemes

### Artic V1
https://github.com/artic-network/primer-schemes/tree/master/nCoV-2019/V1

### Artic V2
https://github.com/artic-network/primer-schemes/tree/master/nCoV-2019/V2

### Artic V3
https://github.com/artic-network/primer-schemes/tree/master/nCoV-2019/V3

### Artic V4
Updated primer-scheme designed by the Artic team. [More info here](https://github.com/artic-network/primer-schemes/tree/master/nCoV-2019/V4)

### Artic V4.1
Minor update (spiked in primers) for the Artic V4 scheme to better recover Omicron ([source](https://github.com/artic-network/artic-ncov2019) and [description](https://community.artic.network/t/sars-cov-2-v4-1-update-for-omicron-variant/342))

### Freed 1.2kb amplicon
Also called the midnight or V1200 primer scheme

https://www.protocols.io/view/sars-cov-2-tailed-amplicon-illumina-sequencing-bge5jtg6

https://academic.oup.com/biomethods/article/5/1/bpaa014/5873518

### Freed 1.2kb amplicon V2 NML
NML adapted primer scheme with minor changes to address Omicron amplicon dropouts

### Resende 2kb amplicon
https://www.protocols.io/view/long-reads-nanopore-sequencing-to-recover-sars-cov-bfy7jpzn

https://www.biorxiv.org/content/10.1101/2020.04.30.069039v1.full.pdf

### Resende 2kb amplicon v2
Small in house modification to Primer 2_F 5’-CTGCTCAAAATTCTGTGCGTGT changing it to Primer 2_F_alt2 5’-ACTCTTGAAACTGCTCAAAATTCTGTG resulting in slightly different schemes and amplicons
