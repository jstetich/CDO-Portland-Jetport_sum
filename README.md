# Portland Jetport Climate Data Analysis
<img
    src="https://www.cascobayestuary.org/wp-content/uploads/2014/04/logo_sm.jpg"
    style="position:absolute;top:10px;right:50px;" />

Data analysis archive for analyzing the eighty year history of weather 
observations at the Portland Jetport.

# Statement of Purpose
CBEP is committed to the ideal of open science.  Our State of the Bay data
archives ensure the science underlying the 2020/2021 State of Casco Bay report
is documented and reproducible by others. The purpose of these archives is to
release  data and data analysis code whenever possible to allow others to
review, critique, learn from, and build upon CBEP science.

# Archive Structure
CBEP 2020/2021 State of the Bay data analysis summaries contain a selection of 
data,  data analysis code, and visualization code as used to produce 
results shared via our most recent State of Casco Bay report. Usually, these
archives are organized into two or three folders, including the following:

- `Data`  folder.  Contains data in simplified or derived form as used in our
data  analysis.  Associated metadata is contained in related Markdown documents,
usually `DATA_SOURCES.md` and `DATA_NOTES.md`.

- Analysis.  Contains one or more R Notebooks proceeding through the principal
data analysis steps that underpin SoCB reporting. To simplify the archives,
much preliminary analysis, and many analysis "dead ends" have been omitted. 

- Graphics.  Contains R Notebooks stepping through development of graphics, and
also copies of resulting graphics, usually in \*.png and \*.pdf formats.  These
graphics may differ from graphics as they appear in final State of the Bay
graphical layouts. Again, most draft versions of graphics have been omitted for 
clarity.

# Summary of Data Sources
All data are derived from data available from NOAA National Centers for
Environmental Information (NOAA NCEI).  Raw data were downloaded from NOAA's
online repositories using a Python script using a Public NOAA API.  Details are
included in a "DATA_SOURCES.md" file in the "Data" folder.

We principally used two different data sets, both accessed through the API.

- GHCND.  Global Historical Climatology Network Daily; Daily data; used here to 
derive length of the growing season, and number of very large storm days 
(> 2 inches of rain) each year.

- GSOY (Global Summary of the Year; Yearly Summaries; used here for all other 
metrics).
