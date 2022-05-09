# Analytical-work

Hi there, if you're reading this it is because you are trying to make sense of the incomprehensible code you saw in 
another file. Well, I'm sorry to tell you that this file will only help you understand about 5% of what the code 
actually does. The code uses data from : the WTO( wto_data.csv) on trade tariffs,
Word Bank (subsidies.csv, subsidies_monetary.csv) for subsidies as a share of government expenses and monetary subsdies
the oecd (PScT_oecd_all.csv , PSE-TSE.csv).


The R code file provides the code used to create, clean, modify and merge the different datasets that can also be found,
as files on my page. The IDB master data was two big to add here but it can be dowloaded 
there -> https://mydata.iadb.org/Agriculture-and-Rural-Development/IDB-Agrimonitor-PSE-Agricultural-Policy-Monitoring/2dqw-u35p


The code structure is as is:

1. Cleaning and creating OECD-AGRIMON dataset on agriucultural support to sugar and meat
a. Filtering, cleaning and modifying variable names of from the IDB master file dataset
b. Modifying variable names to from the OECD dataset that was compiled manually on excel from the OECD
c. Merge the two data sets in longer format
d. Make a "MEAT" variable to be compatible with GDD data

2. Descriptive graphs to show what information we have depending on commodities, countries and year
Basically seeing how many countries produce each commodity, the time span, level of support and whatnot.

3.Find the relationship between total subsidies and Ag support
Here we compare support to agriculture for OECD and Agrimon countries (PSE-TSE.csv) and total subsidies (subsidies.csv)
which is used by Abbay in order to see if it brings something new to the analysis.
An important modification here is that we compare support to agriculture as a share of government expenses.
Because the World Bank does not provide information on that explicitly, we infer it by using the monetary amount
of support with the subsidies_monetary.csv file.
Several graphs are created here to look at the correlation.

4. WTO and Subsidies data to create datasets to reproduce findings from abbay
I)
We then use the wto data on tariffs (wto_data.csv) and information on total subsidies as % of governement expenses
to create a new data set with only the countries present in the OECD-Agrimon dataset in order to reproduce the findings
from Abbay with only our select countries.

II) 
The same thing is with countries specifically studies by abbay in their paper for reproduction purposes.









