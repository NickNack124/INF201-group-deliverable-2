# INF201-group-deliverable-2
A shared repository for the purpose of completing the second 2-week group assignment in INF201.

# Requirements
This code necessitates the existance of a folder in the same workspace by the name of "data", containing:
  * at least 1 .log file containing transaction information from one or more cash registers
  * at most 1 .json file containing metadata on these registers
    * This file must contain a json dictionary, in which there must exist a sub-dictionary with
      at least the (key, value)-items: (key="id", type(value) is str) and (key="active", type(value) is bool)

The necessary packages can be found in the "requirements.txt" file

# The premise
This data is from several cash registers located at different places throughout a campus.
These logs include information on a register's location, as well as each of their recorded transactions.
These transactions include data on the time of each transaction, what was bought, what currency was used, which register was used, etc

# Products
The notebook in this repository is intended to produce 4 files;
  * "cleaned_transactions.csv" (containing cleaned up data about the transactions)
  * "hourly_revenue.json" (a .json dictionary containing the hourly revenue for each item)
  * "status_pivot_table.csv" (a .csv file containing data on each item, aggregated based on register-statuses)
  * "item_refund_ratios.csv" (a .csv file containing the refund ratios of their respective sold items)
