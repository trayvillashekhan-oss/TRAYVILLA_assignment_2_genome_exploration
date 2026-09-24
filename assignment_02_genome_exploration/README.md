# Genome Exploration II

**Name:** Shekhan Fredianne C. Trayvilla  
**Activity:** Basic Genome Structure and Sequence Exploration Using Galaxy  
**Genome:** Anas strepera (the FASTA header uses Mareca strepera)  
**NCBI assembly accession:** To be confirmed from the original NCBI assembly page  
**Original Galaxy dataset:** `Anas_strepera_genome_original.fna.gz.gz`  
**Original file size in Galaxy:** 383.8 MB  
**Galaxy History:** https://usegalaxy.org/histories/view?id=bbd44e69cb8906b56089316a64f25f43

## Objective

I examined the structure of the genome assembly used in my previous assignment. I calculated assembly statistics, sorted its sequences by length, and compared the original assembly with a copy containing sequences at least 10,000 bp long.

## Tools and steps

1. **gfastats:** Calculated assembly statistics for the original genome FASTA (Galaxy dataset 1; statistics in dataset 2).
2. **Compute sequence length:** Calculated the length of each FASTA sequence (dataset 3).
3. **Sort:** Sorted the sequence-length table from longest to shortest (dataset 7).
4. **Filter sequences by length:** Kept sequences at least 10,000 bp long in a copy of the original FASTA (filtered copy in dataset 4).
5. **gfastats:** Calculated statistics for the filtered copy (datasets 5 and 9).

The original FASTA was retained. The original and filtered statistics are compared in `results_table.md`.

## Main findings

The original assembly contains 1,156 scaffolds totaling 1,300,614,387 bp. Its largest scaffold is 205,626,557 bp, scaffold N50 is 66,097,916 bp, scaffold L50 is 6, and GC content is 42.39%.

The 10 kb filter retained 1,104 scaffolds totaling 1,300,429,993 bp. It removed 52 short scaffolds totaling 184,394 bp, about 0.014% of the original assembly length. The scaffold N50 and L50 stayed the same because the removed scaffolds contributed very little to the total length. Filtering was an exercise for examining the assembly; it does not automatically make the genome better.

The five longest sequences are listed in `results_table.md`.

## ORF exploration status

I used ORFipy to examine one 2,000 bp sequence from the Anas strepera assembly. Using the standard genetic code, both strands, and a minimum ORF length of 150 nucleotides, the tool found 11 candidate ORFs. These are predicted regions, not confirmed genes.

## Evidence

- [Small-region ORF results](screenshots/small_region_orfs.png)
- [ORFipy settings](screenshots/small_region_orf_settings.png)

## Evidence

- [Galaxy history](screenshots/galaxy_history.png)
- [Original genome preview](screenshots/original_genome.png)
- [Original genome details](screenshots/original_genome_details.png)
- [Original assembly statistics](screenshots/original_statistics_1.png)
- [Original GC content](screenshots/original_statistics_2.png)
- [Longest sequences](screenshots/longest_sequences.png)
- [Filtered assembly statistics](screenshots/filtered_statistics_1.png)
- [Filtered GC content](screenshots/filtered_statistics_2.png)

