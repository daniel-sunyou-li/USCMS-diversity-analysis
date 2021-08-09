# USCMS-diversity-analysis
A collection of Python notebooks visualizing the diversity of members within the CMS and USCMS collaboration. Notebooks are indicated whether they should be run on Google Colaboratory or on CERN's [SWAN notebook service](cern.swan.ch). For each notebook, the relevant `json` data files should all be contained within the subdirectory `USCMS-diversity-analysis/Data/` and are up to date as of __August 9th, 2021__.  When using the Google Colaboratory notebooks, be sure to edit the `%cd` command to use your working directory.  Everything else should be "plug and play" based on a GUI.

The notebooks `authors_per_institute_*.ipynb` [[Colab](https://github.com/daniel-sunyou-li/USCMS-diversity-analysis/blob/main/authors_per_institute_colab.ipynb)/[SWAN](https://github.com/daniel-sunyou-li/USCMS-diversity-analysis/blob/main/authors_per_institute_swan.ipynb)\] produce a stacked bar graph grouped by institution showing the number of affiliated men and women per year.  

The notebook `combine_json_*.ipynb` [[Colab](https://github.com/daniel-sunyou-li/USCMS-diversity-analysis/blob/main/combine_json_colab.ipynb)/[SWAN](https://github.com/daniel-sunyou-li/USCMS-diversity-analysis/blob/main/combine_json_swan.ipynb)] consolidates the various `json` files in `Data` into a single combined `json` file that can be used for further analysis.  The format of the `json` is that for each year, there is a `dict` of CMS IDs containing the following information: `AUTHOR` (`True` or `False`), `GENDER`, `PROJECT`, `ACTIVITY` and `INSTITUTE`. 

The notebook `cms_statistics_*.ipynb` [[Colab](https://github.com/daniel-sunyou-li/USCMS-diversity-analysis/blob/main/cms_statistics_colab.ipynb)/[SWAN](https://github.com/daniel-sunyou-li/USCMS-diversity-analysis/blob/main/cms_statistics_swan.ipynb)] takes the consolidated `json` file from `combine_json_*.ipynb` and reports filtered statistics.

The notebook [`gender_per_activity_colab.ipynb`](https://github.com/daniel-sunyou-li/USCMS-diversity-analysis/blob/main/gender_per_activity_colab.ipynb) shows the gender distribution for the various research activities (i.e. 'Doctoral Student', 'Physicist', etc.) per year.  

The notebook [`gender_per_age_colab.ipynb`](https://github.com/daniel-sunyou-li/USCMS-diversity-analysis/blob/main/gender_per_age_colab.ipynb) produces two plots:
* The gender distribution for each age group for the CMS or USCMS researches by periods of years (i.e. between 1995-2003, 2004-2012, etc.)
* The gender ratio for each age group per birth year cohort

The notebook [`gender_per_region_colab.ipynb`](https://github.com/daniel-sunyou-li/USCMS-diversity-analysis/blob/main/gender_per_region_colab.ipynb) shows the gender distribution for each region (i.e. 'CERN', 'RDMS', 'USCMS', etc.) for a given period of years.  

The notebook [`leadership_by_gender_colab.ipynb`](https://github.com/daniel-sunyou-li/USCMS-diversity-analysis/blob/main/leadership_by_gender_colab.ipynb) plots the gender distribution for the various leadership roles within L1 and SP Team, L2 POG and L2 PAG.  It also produces a table of the USCMS institutes represented in CMS leadership funded by 'NSF CA' for a given period and shows the gender distribution.  

The notebook [`visualize_publications_swan.ipynb`](https://github.com/daniel-sunyou-li/USCMS-diversity-analysis/blob/main/visualize_publications_swan.ipynb) shows two types of plots:
* A (non-stacked) histogram of the gender-split author count versus the number of presentations given in the past 3 years.
* A 2D-histogram of the number of author presentations versus years spent in the colaboration, wiht separate histograms provided for 'Male' and 'Female' data
