# The Olympic Games - What factors impact on medal counts and which countries can we expect to do well in Paris 2024?


For this project, I created a Tableau storyboard which explores the medal tally of countries around the world since the __year 2000__, and how different geopoltical, social and economic factors can influence performance in the games. I then used the Tableau function __MODEL_QUANTILE__ to experiment with predicting the likely range of medals each country will be awarded in the upcoming Paris 2024 games. 🔵 🟡 ⚫ 🟢 🔴

## Tableau Public 🏞️

You can find the final storyboard [here](https://public.tableau.com/app/profile/jade.soanes7422/viz/Olympics_FINAL/OLYMPICSSTORYBOARD) on Tableau Public!

If you enjoy the project please consider nominating it for __Viz of the Day__!

## Test It For Yourself ✏️

You can find the Tableau file and csv data files in this repo (zipped). To try out this viz for yourself simply download the files, save them all in one place and load up Tableau desktop. When you open the Tableau file you will be asked to reconnect to the datasources - just select the relevant file names when prompted.

All data files are .xslx or .csv

The PNG files for the images in the dashboard are also saved in the zip file.

## The Details 🧐

### Data

* Limited analysis to show only Olympics held from the year 2000. This is because of changing geopolitics in the 1990s meaning a lot of historic countries no longer exist!
* Normalised a lot of the data to be __per person/number of people__, for example medals per 10M people or GDP per person. This is so population does not skew the analysis of the other factors.
* However this normalisation did come with some drawbacks, namely small countries and terrorories creating anomalous results. An example of this is San Marino, a nation taht has only won two medals since the year 2000, however because of its small population this is normalised to +100 medals per 10 M people per games - which is not sensible! Therefore the medals per 10M people measure has been capped at 20, where 98% of the results lie below.

### Visuals

* Aimed to put a lot of the detail in to the tooltips to keep the main visuals easy to read and tidy.
* Used the Tableau colour-blind friendly colour palette.

### Modelling

* Predicting the medal count per country using historic data about GDP, Population, Military Spending and Education Spending.
* The modelling does not take 2024 specific factors into account, e.g., France potentially gaining a host country advantage.
* Russia and Belarus are excluded from the modelling as athletes are banned from entering under either country's banner in Paris 2024.

## Datasets and Sources :open_book:

* [Olympic medals and host data - Kaggle](https://www.kaggle.com/datasets/heesoo37/120-years-of-olympic-history-athletes-and-results)
* [GDP data - The World Bank](https://data.worldbank.org/indicator/NY.GDP.MKTP.CD?end=2022&amp;most_recent_year_desc=true&amp;start=1960&amp;view=chart)
* [Education spending data - The World Bank](https://data.worldbank.org/indicator/SI.POV.DDAY?locations=1W&amp;name_desc=true&amp;start=1984&amp;view=chart)
* [Population data - The World Bank](https://data.worldbank.org/indicator/SP.POP.TOTL?view=chart)
* [Military spending data - The World Bank](https://data.worldbank.org/indicator/MS.MIL.XPND.GD.ZS)
* [Natural disasters data - Our World in Data](https://ourworldindata.org/natural-disasters)
