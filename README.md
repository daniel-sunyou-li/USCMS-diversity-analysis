# USCMS-diversity-analysis
A collection of Python notebooks visualizing the diversity of members within the USCMS collaboration

The notebooks `authors_per_institute_*.ipynb` produce a stacked bar graph grouped by institution showing the number of affiliated men and women per year.  

The notebook `combine_json_*.ipynb` consolidates the various `json` files in `Data` into a single combined `json` file that can be used for further analysis.  The format of the `json` is that for each year, there is a `dict` of CMS IDs containing the following information: `AUTHOR` (`True` or `False`), `GENDER`, `PROJECT`, `ACTIVITY` and `INSTITUTE`. 

The notebook `cms_statistics_*.ipynb` takes the consolidated `json` file from `combine_json_*.ipynb` and reports filtered statistics.
