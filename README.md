**Author**: Swetha Yadavalli

**Programming Language**: Python

**Dependencies**:
- pandas
- numpy

**Files required**:
- argR-counts-matrix.txt
- E_coli_K12_MG1655.400_50

## Description

This script involves analyzing gene sequences to identify potential binding sites using a Position Weight Matrix (PWM). The scripts process gene sequence data and PWM information to calculate similarity scores and identify the top 30 genes with the highest similarity to the PWM.

## Execution Steps

1. All of the necessary libraries should be loaded in the python environment. 
2. The script reads base counts from argR-counts-matrix.txt 
3. These counts are then transformed into a frequency matrix.
4. The frequency matrix is converted into a PWM by calculating the log ratio against the background frequency of each base.
5. Gene sequences are then read from E_coli_K12_MG1655.400_50.
6. Each line is split to extract the GeneID and the corresponding sequence.
5. The script iterates through each gene's sequence and calculates the similarity score for all possible subsequences matching the PWM length.
6. For each sequence, the highest score is identified and are used to determine the gene's binding site similarity to the PWM.
7. The genes are sorted by their maximum scores and top 30 genes with the highest scores are selected and listed.

## Output Files

The final .pynb can be accessed for the IDs of the top 30 genes as the output. 
