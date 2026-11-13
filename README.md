# WP8_PT_DMR

Monthly Remuneration Declaration detection of Editing needs using ML

Monthly Remuneration Declaration dataset is received monthly from Social Security around the 18th. It contains information about the previous four months; versions n-1 to n-4. The companies can submit in the following months another version of the data and it’s assumed that the accuracy improves in the latest version.
The possibility to submit a later and different value for the data impacts the process of data collection. It can create an apparent significant change in a month's data that is actually a result of a reporting lag from the previous month. This catch-up effect can create misleading spikes or jumps in the dataset that we would like to avoid.
The obvious solution is imputing. However, this may create an additional problem imputing values in cases where they should in fact be left blank. So, the question we want to address using ML is to support us in the decision of imputation. For missing data, is it really missing or not.  For reported data will it be changed later on and should we impute a value that could minimize the gap.
