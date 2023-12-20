# Challenge4
## I: Summary
### Procedure
While Power BI has its strengths, we decided that searching for the most effective policies would be easiest using python.
- We created a variable named `Measure` in Power BI, which is the proportion "`Confirmed_Change` (newly confirmed cases over the past week) divided by `Current_Cases` (cases that are currently active)". We have also considered calling this **Growth Rate Index** given its nature.
- After adding `Measure` to a table alongside many columns from the table "Policies", we exported the table to a csv file.
- Using the csv file, we performed **linear regression** with Python (and with help from `scikit-learn`).
### Results
- We are basing our conclusion on the coefficients of our linear regression models.
- **The three most effective policies** were:
    - school closing: no measures
    - public events: require cancelling
    - public information campaigns: coordinated information campaign
- Of our assigned policies, we believe that:
    - 'public information campaigns: coordinated information campaign' was effective
    - 'public events: recommend cancelling' was less effective than outright *cancelling* public events.
