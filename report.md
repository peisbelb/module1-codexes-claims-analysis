Errors encountered during the analysis:
With the help of the repo titled wk1_helperStarter_code.py, it was easy to go through each step and understand the parts that needed to be conducted. 
However, I ran into issues when understanding the names of certain columns and what each column was showing. In the example shown in the repo provided by the professor, it didn't match the exact names shown in the inpatient data set which threw me for a bit of a loop.
I had trouble with finding the frequencies, so I used code that was provided by a classmate on Teams: 


codex_columns = [
    'PRNCPAL_DGNS_CD',
    'ICD_DGNS_CD1',
    'ICD_PRCDR_CD1',
    'CLM_DRG_CD',
    'ADMTG_DGNS_CD',
    'HCPCS_CD',
    'FST_DGNS_E_CD',
    'NCH_DRG_OUTLIER_APRVD_PMT_AMT'
]
for column in codex_columns:
    print(f"Frequency counts for {column}:")
    value_counts = df[column].value_counts()
    print(df[column].value_counts())
    print("\n")

 
 In using this particular code, I was able to find the frequencies for ICD,DRG, and HCPCS codes.
    
 However, after reviewing the repo provided by the professor, I was able to find the frequency through his method. I think I was initially getting confused on whether to use the name of the columns provided in the data set or the name I established for the columns.

Example: whether to use icd_codes or ICD_DGNS_CD1 when trying to find frequencies. 


 After establishing which was the correct coding to use, I was able to find the frequencies. On my end, I had no missing values. 
 
 Truthfully, it is a little hard for me to interpret the data and its meaning. I was able to follow the steps provided by the professor, but to understand the data and be able to retrieve it myself with no additional material or support would be a challenge. 
