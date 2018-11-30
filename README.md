# Early genomic detection of the Cosmopolitan Genotype of Dengue Virus 2 in Angola, 2018

This folder contains raw and processed sequencing data related to the sequencing of a Cosmopolitan genotype dengue 2 virus in Angola, Luanda. The protocol used for sequencing is explained in detail in the publication ‘Early genomic detection of the Cosmopolitan Genotype of Dengue Virus 2 in Angola, 2018’, by Hill et al. This is currently under review. Please note that the data here include the positive sample, and two different negative controls that were processed and sequenced along with the positive sample (including a water control extracted with the dengue sample and an additional water control introduced at cDNA synthesis).

Files are named according to file type and barcode. Pool A and Pool B refer to the PCR primer pool used to conduct amplification (see Quick et al. Nature Protocols volume 12, pages 1261–1276 (2017) for details). The barcodes, identifiable by ‘BCXX’ at the start of each file name, are as follows:

## Barcodes

- BC01: Extraction negative control (H20), Pool A 
- BC02: Extraction negative control (H20), Pool B
- BC03: cDNA synthesis negative control (H20), Pool A
- BC04: cDNA synthesis negative control (H20), Pool B
- BC05: Positive dengue 2 sample, Pool A
- BC06: Positive dengue 2 sample, Pool B

## File types
The file types are identifiable by the suffix of the file name. Specifically, file types are:

- `.fast5`: Demultiplexed raw reads from that barcode (only available under [releases](releases/))
- `.fasta`: Basecalled reads from that barcode 
- `.sorted.bam`: bwa mapped BAM file of basecalled reads for each barcode, sorted using samtools 
- `.trimmed.sorted.bam`: BAM file trimmed to the external of each primer (i.e., primer regions retained)
- `.primertrimmed.sorted.bam`: BAM file trimmed to the internal of each primer (i.e., primer regions removed).
- `.vcf`: VCF file of variants to reference sequence from that barcode (GenBank accession: LC121816)
- `.consensus.fasta`: Consensus sequence from that barcode (please note, Pools A and B from each sample must be combined to get ‘final’ FASTA file for that sample, as each PCR pool only amplifies half the genome). 

We also provide input references genomes and BED files that were used as inputs to the pipeline, with prefixes 'DENV2_90consensus' being generated from the 90% consensus of a DENV2 alignment, and 'DENV2_LC121816' being generated from the highest identity sequence (GenBank Accession number LC121816). Please see Technical Appendix of our submitted paper for details. 

# Authors:

_Sarah C Hill (1), Jocelyne Neto de Vasconcelos (2), Bernardo Gutierrez Granja (1,3), Julien Thézé (1), Domingos Jandondo (2), Zoraima Neto (2), Marinela Mirandela (2), Cruz dos Santos Sebastião (2), Ana Luísa Micolo Cândido (2), Carina Clemente (5), Sara Pereira da Silva (5), Túlio de Oliveira (4), Oliver G Pybus (1), Nuno R Faria (1), Joana Morais Afonso (2)_

1. University of Oxford, Oxford, UK.
2. Instituto Nacional de Investigação em Saúde, Luanda, Angola.
3. Universidad San Francisco de Quito USFQ, Colegio de Ciencias Biológicas y Ambientales, Quito, Ecuador.
4. University of KwaZulu-Natal, Durban, South Africa
5. Cligest, Luanda, Angola

# Abstract of the work (under review)
We used portable genome sequencing to investigate reported dengue virus transmission in Angola. Our results reveal autochthonous transmission of dengue serotype 2 (Cosmopolitan genotype) in Jan 2018.