Jupyter notebook to get the SciMago-indexed psychology journals to filter PubMed abstracts by psychology domain: "2_pubmed_SM_matched_journals.csv".

# What it does:
- From the unique list of 1,376 SciMago-indexed psychology journals, the jupyter notebook matches journal titles from this list with the 53,349 journals in PubMed (#1), yielding 583 SciMago classified journals (#2). There were no cases where the same journal id was matched with different subject categories. 
- The final key file of this script (renamed to "psy_journals_list.csv") is used to filter parsed PubMed data in https://github.com/Zendelo/PubMedParse to get a corpus of Pubmed psychology abstracts.

# More detail:
Note: 404 rows where duplicates appear as the same journal is indexed in more than one SciMago category (based on Sourceid)/ 

Final `Subject_Category_SciMago` 623 journals
- Developmental_and_Educational_Psychology         148 
- Social_Psychology                              	 138 
- Clinical_Psychology                            	 116 
- Psychology_(miscellaneous)                    	 105 
- Applied_Psychology                               59 
- Experimental_and_Cognitive_Psychology        	   38 
- Neuropsychology_and_Physiological_Psychology     19 

Note: Decision to exclude journals including articles published in a language other than English, leaving 1,169 journals, was redacted to filter at a later stage (after the PubMed corpus is compiled).

Footnote: 
- #1: Link to PubMed journals (accessed April 2024): https://ftp.ncbi.nih.gov/pubmed/J_Medline.txt
- #2: Link to SciMago classified psychology journals (accessed April 2024): https://www.scimagojr.com/journalrank.php?area=3200  

Example of pubmed journal chunks

JrId: 2 \\
JournalTitle: AANA journal \\
MedAbbr: AANA J \\
ISSN (Print): 0094-6354 \\
ISSN (Online): 2162-5239 \\
IsoAbbr: AANA J \\
NlmId: 0431420 \\
