The goal of this question is to assess the candidate's familiarity with sequence algorithms and Python programming skill.  Accordingly there are several levels to the solution of this problem.  

# Problem description

Input: 

- $3^{\prime}$ scaffold sequence: GTTTAAGAGCTAAGCTGGAAACAGCATAGCAAGTTTAAATAAGGCTAGTCCGTTATCAACTTGAAAAAGTGGCACCGAGTCGGTGCTTTTTTT;
- Promoter sequence: TTTTTTG;
- text file of spacer sequences: `guide_RNA_seq.txt`;
- fastq files of sequenced guide RNAs: `sequenced_guides.fastq`.   We can assume that we are only working with the actual sequence parts of the fastq files and ignore quality scores.

A sequenced guide RNA should (in theory) have the promoter sequence followed by the spacer sequence, then the $3^{\prime}$ scaffold sequence, flanked on other sides by other stuff. This other stuff doesn't matter but is sequenced anyways because the length of the scaffold + space is much smaller than the length of a standard read. 

The goal of the problem is to produce a count of the number of times each spacer is sequenced.  Note that each sequenced read should only have one spacer.