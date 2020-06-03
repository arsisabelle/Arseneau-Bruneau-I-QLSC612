# Arseneau-Bruneau-I-QLSC612
Assignment of Week 1 of BHS

Requirements and Virtual Environment

For this analysis, we assume that you have Conda environment installed on your computer. (If this is not the case, go to https://docs.conda.io/projects/conda/en/latest/user-guide/install/ )
 

To facilitate the installation of the dependencies, a virtual environnement has been created so users can avoid troubles experienced on local machines by the author of this notebook). Thus, make sure to follow the installation instructions described here, on in the README.md document, and at the beginnind of the jupyter notebook of this repository.

To Install and run the virtual environment, go to your terminal and enter the following commands:

`conda env create --file isabelle.yml`

`conda activate isabelle`

`jupyter notebook myAnalysis.ipynb`

The codes of this notebook uses the following dependencies:
- python=3.7
  - matplotlib
  - numpy
  - pandas
  - scipy
  - notebook
  - statsmodels


RESEARCH DESCRIPTION

We are interested to see if the number of social conflicts experienced by participants during a segment of the COVID-19 confinement (y-variable 'partY') may have been influenced by several factors, such as the participant's Gender, their Verbal IQ, their brain volume (MRI_Count), or their alchool intake during the corresponding period (y-variable 'partY2').

'partY' is measured as the number of conflicts reported during the 6th week of the COVID confinement
'partY2' is measured as the number of standard alchool intake (as defined by Educalcool, for details see reference below) reported by participants for the period covering the 6th week of the COVID confinement

(Éduc’alcool (Association). (2007). Alcool et santé: Les niveaux de consommation d’alcool à faible risque, 2-3-4-5-0. Éduc’Alcool.)

Statistical analysis where conducted on "My-super-Macbook-Pro-that-fits-in-an-envoloppe" with the software packages described above, in the Amazing virtual environment mentioned above. We performed Independant sample t-tests and OSL requressions, we provided bicolore scatterplot figures and boxplot to illustrate these results. The results suggest a possible interraction effect (intercept) of gender on alchool intake (partY2), when examined in relation to social conflicts experienced during the 6th week of confinement and verbal IQ. 

As the analysis met several conditions for p-hacking (rejection of subject with incomplete data, male sample size <20 [n =18],no mention of all of the analysis performed, multiple comparaisons computed and presented in the results as only one single comparaison [that is bad statistical practices!], no application of correction or adjustments of the degree of freedom in multiple comparaisons, results of the OLS Regression reporting only the significant results rahter than 3 models), we conclude that our current findings may not allow us to conclude anything regarding the relationships of x-variables verbal IQ, brain volume, gender, or gender interactions, with the amount of social conflicts (partY) and alchool intake (partY2) experienced during the 6th week of COVID-19 confinement. Thus, stay sane, drink with fun and moderation, and happy Brainhacking!
