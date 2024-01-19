# Guide to files in `Notebooks` folder

The post peptide/protein ID parts of the data analysis are done using [Jupyter notebooks](https://jupyter.org/), the [R language](https://www.r-project.org/), and Bioconductor packages [edgeR](https://www.bioconductor.org/packages/devel/bioc/vignettes/edgeR/inst/doc/edgeRUsersGuide.pdf) and [limma](https://www.bioconductor.org/packages//2.11/bioc/vignettes/limma/inst/doc/usersguide.pdf). An overview of Jupyter notebook use in proteomics can be found here: https://github.com/pwilmart/Cascadia_2018. More details on how to set up an R kernel for Jupyter notebooks can be found here: https://github.com/pwilmart/R-Jupyter-notebook_setup.

The notebook files (`*.ipynb`) can be viewed directly at GitHub. The extension is short for iPython Notebook (ipynb). The iPython shell and the JSON format for the notebook files predates the Jupyter project. When you have Jupyter, python, and R installed on your computer, and have configured an R kernel for notebooks, the notebook files will be "live". The cells can be changed and re-run. That takes some effort to set up. Viewing the notebooks using the GitHub interface is a lot easier.

If you download the file to your computer (either as a Zip archive or by cloning the repository with Git), you lose the GitHub notebook rendering feature. Each notebook has been saved as an HTML file that can be viewed with any browser. These are static snapshots of the notebooks.

## Notebooks and descriptions:

- `Khan-2018_QC_checks.ipynb` and `Khan-2018_QC_checks.html`
  - Notebooks that look at variety of quality control data aspects.
- `Khan-2018_edgeR-ANOVA_TMM.ipynb` and `Khan-2018_edgeR-ANOVA_TMM.html`
  - Notebooks that perform one-way ANOVA on TMM-normalized data. The general linear modeling features of edgeR are used. Benjamini-Hochberg multiple testing corrections are applied.
- `Khan-2018_edgeR-ANOVA_noTMM.ipynb` and `Khan-2018_edgeR-ANOVA_noTMM.html`
  - Notebooks that perform one-way ANOVA on data without using TMM normalization (grand total normalized only). The general linear modeling features of edgeR are used. Benjamini-Hochberg multiple testing corrections are applied.
- `Khan-2018_edgeR-E15-E18P0-P3P6-exact_TMM.ipynb` and `Khan-2018_edgeR-E15-E18P0-P3P6-exact_TMM.html`
  - Notebooks that compare E15 to E18/P0 ages, or compare E18/P0 to P3/P6 ages. The data has been TMM normalized. The pair-wise comparisons use the edgeR exact test, experiment-wide trended variance, and Benjamini-Hochberg multiple testing.
- `Khan-2018_edgeR-successive-ages-exact_TMM.ipynb` and `Khan-2018_edgeR-successive-ages-exact_TMM.html`
  - Notebooks that compare each pair of successive ages (E15 to E18, E18 to P0, P0 to P3, P3 to P6, and P6 to P9). The data has been TMM normalized. The pair-wise comparisons use the edgeR exact test, experiment-wide trended variance, and Benjamini-Hochberg multiple testing.
- `Khan-2018_edgeR-successive-ages-exact_noTMM.ipynb` and `Khan-2018_edgeR-successive-ages-exact_noTMM.html`
  - Notebooks that compare each pair of successive ages (E15 to E18, E18 to P0, P0 to P3, P3 to P6, and P6 to P9). The data has been grand total normalized only (no TMM). The pair-wise comparisons use the edgeR exact test, experiment-wide trended variance, and Benjamini-Hochberg multiple testing.
- `Khan-2018_edgeR-young-old-exact_TMM.ipynb` and `Khan-2018_edgeR-young-old-exact_TMM.html`
  - Notebooks that compare the two youngest ages (E15 and E18) to the two oldest ages (P6 and P9). The data has been TMM normalized. The pair-wise comparison uses the edgeR exact test, experiment-wide trended variance, and Benjamini-Hochberg multiple testing corrections.
- `Khan-2018_edgeR-young-old-exact_noTMM.ipynb` and `Khan-2018_edgeR-young-old-exact_noTMM.html`
  - Notebooks that compare the two youngest ages (E15 and E18) to the two oldest ages (P6 and P9). The data has been grand total normalized only (no TMM). The pair-wise comparison uses the edgeR exact test, experiment-wide trended variance, and Benjamini-Hochberg multiple testing corrections.

**Output files written by the notebooks:**
- `Khan-2018_results_3-age-groups_edgeR-exact_TMM.txt`
  - E15 versus E18/P0 and E18/P0 versus P3/P6 comparisons with TMM
- `Khan-2018_results_edgeR-ANOVA_TMM.txt`
  - ANOVA results with TMM
- `Khan-2018_results_edgeR-ANOVA_noTMM.txt`
  - ANOVA results without TMM
- `Khan-2018_results_edgeR-exact_TMM.txt`
  - E15/E18 versus P6/P9 with TMM
- `Khan-2018_results_edgeR-exact_noTMM.txt`
  - E15/E18 versus P6/P9 without TMM
- `Khan-2018_results_successive-ages_edgeR-exact_TMM.txt`
  - Comparisons between successive ages with TMM
- `Khan-2018_results_successive-ages_edgeR-exact_noTMM.txt`
  - Comparisons between successive ages without TMM
