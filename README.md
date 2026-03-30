5004CMD — BTS Mobility Analysis

Coursework repository: Word report, notebook workflow, datasets, timings, and figures.

Repository:
github.com/Hotphot/5004CMD-Data-Science

Contents

File / folder | Description
5004CMD_Project_Report.docx | Final report with methodology, modelling results, and runtime evaluation.
5004.ipynb | Main notebook containing preprocessing, aggregation, regression modelling, plots, and execution timing comparison.
Trips_by_Distance.csv | National mobility dataset across distance bands.
Trips_Full Data.csv | Week 32 distance distribution dataset.
timing_results.csv | Serial vs parallel runtime comparison.
figures/ | Six generated figures used in the report.

Setup

Install required packages before running the notebook:

pip install pandas numpy matplotlib scikit-learn dask distributed pyarrow

Run

Launch the notebook:

jupyter notebook 5004.ipynb

If converted to script form:

python analysis.py

On Windows, if Matplotlib errors occur:

$env:MPLBACKEND="Agg"; python analysis.py

Clone repository

git clone https://github.com/Hotphot/5004CMD-Data-Science.git

cd 5004CMD-Data-Science

Project summary

This coursework analyses national travel behaviour using the Bureau of Transportation Statistics Daily Mobility Statistics dataset. The workflow investigates stay-at-home trends, distance-based mobility structure, threshold exceedance periods, regression relationships between trip length and frequency, and runtime performance differences between sequential and distributed processing pipelines.

Sequential Pandas and parallel Dask workflows execute identical analytical steps so performance differences reflect execution strategy rather than modelling changes.

Figures generated

The figures directory contains:

Figure 1. Weekly stay-home trend
Figure 2. Week 32 distance distribution
Figure 3. Threshold exceedance scatterplot
Figure 4. Polynomial regression fit
Figure 5. Average distance-band mobility
Figure 6. Runtime comparison
