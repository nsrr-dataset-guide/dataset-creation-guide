# Import an Existing Data Dictionary

If you already have a data dictionary for a study in a CSV format, Spout can import the existing variable information into the data dictionary it creates. If you would like to import a preexisting data dictionary, simply do the following, in addition to the steps described in [Chapter 4.2.1](data_dictionaries/create_a_new_data_dictionary.md):

- After creating a new data dictionary using `spout new`, navigate into the data dictionary using `cd example-data-dictionary`
- Once inside of your data dictionary, you can import the CSV file using the spout command `spout import $data_dictionary.csv`, where $data_dictionary.csv is the full file path to the location of your CSV data dictionary.

Many of Spout's features will be discussed in later sections of this guide, but if you run into any issues installing or using Spout, you can find support at the GitHub repository for it: [https://github.com/sleepepi/spout](https://github.com/sleepepi/spout)
