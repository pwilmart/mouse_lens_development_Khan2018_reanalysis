# Guide to files in `Spreadsheets` folder

Large spreadsheets are the way the results are summarized. These sheets include common proteomics data (protein accessions, protein descriptions, sequence coverage, peptide counts, etc.), quantitative data (reporter ion intensities summarized to the protein level), normalized data values, statistical testing results (p-values, FDRs, fold changed, etc.), and some useful annotation information (https://pwilmart.github.io/blog/2019/10/14/orthologs-annotations).

It helps to have multiple large monitors when working with large data tables (or at least one large monitor). They are view features that can help like split views, hiding rows and columns that are not of current interest. Hiding rows/columns is better than deleting data from a data integrity standpoint. You might need to read up on some spreadsheet features and do some practicing before you jump into full on data exploration. See https://pwilmart.github.io/blog/2020/07/24/How-to-Excel for some background.  

## Spreadsheets and descriptions:

- prefix_columns.xlsx
  - A few columns from the PAW protein summary table to have at the left of each sheet.
- Khan-2018_ANOVA_successive-ages_young-old_TMM.xlsx
  - edgeR statistical testing done 3 ways: one-way ANOVA, pairwise test between two youngest ages and two oldest ages, pairwise tests between successive ages with TMM-normalized data.
- Khan-2018_ANOVA_successive-ages_young-old_noTMM.xlsx
  - edgeR statistical testing done 3 ways: one-way ANOVA, pairwise test between two youngest ages and two oldest ages, pairwise tests between successive ages with grand-total-normalized data (no TMM).
- Khan-2018_TMM_extras.xlsx
  - Sheet that uses average intensities for each age to explore proteome characteristics (cumulative abundance) and explore 20 well known lens proteins. The data has been TMM-normalized.
- Khan-2018_labeled_grouped_protein_summary_TMT_9.xlsx
  - Spreadsheet of the IRS script starting data where fractions of the total intensity from  crystallins are computed for each of the 18 samples.
- Khan-2018_results_3-age-groups_edgeR-exact_TMM.xlsx
  - Age groups that were separated on the cumulative distribution plot are compared (E15 versus E18/P0 and E18/P0 versus P3/P6) using TMM-normalized data and edgeR exact test. This sheet also has slope analysis of scaled average intensities (divided by median intensity).
- annotations.xlsx
  - A subset of UniProt protein annotation columns that are added to the right of most of the above sheets. Information includes gene symbols, links to UniProt and MGI, UniProt Keywords, GO terms, and Reactome pathway details.
