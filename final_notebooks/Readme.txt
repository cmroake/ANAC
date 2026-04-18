Instructions on how to use this pipeline. 

Source Table: "_github-AAC_accidents_tagged_data.xlsx"
Route Table: "routes_matcher_combined.csv"

Tagging File 1: "ANAC_addtags_matching.ipynb"
Input: Source Table, Route Table
Output: CSV with tags for location, date, climb type, rope, and helmet

Tagging File 2: "ANAC_llm_unified_pipeline.ipynb"
Input: CSV from the tagging file 1 output, .env variable for API
Output: Fully tagged CSV ("ANAC_final_tags.csv")

Final Analysis: "Final_Combined_Analysis_Reordered_USETHIS.ipynb"
Input: Fully tagged CSV ("ANAC_final_tags.csv")
Output: none

*** IMPORTANT ***
The analysis can be done alone from the "Final_Combined_Analysis_Reordered_USETHIS.ipynb"
and the fully tagged CSV ("ANAC_final_tags.csv")

The tagging codes and intermediate tables are only for modifying tags