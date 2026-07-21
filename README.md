# Azure-Synapse-Analytics
Customer 360 Data Integration

In this project, we are fetching a dataset from the Kaggle website which has a
dataset on Customer 360 Data.
Link to the dataset: https://www.kaggle.com/datasets/varunkumari/customer-360-data
The objective of this project is to clean the datatset and perform SCD Type-2
transformation on them.
We are following a medallion architecture here, where-in, the raw data will be
stored in the bronze layer in ADLSGEn2 in csv format, then the data will be
cleaned and stored in the silver layer in delta format, again in ADLSGen2 and finally, SCD-2
transformations will be performed and business-ready data will be stored in a delta table in the gold
layer. We are also doing the analysis of our tables after creating views on top of the externals tables we
will create form them.
