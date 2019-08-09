# MS-Dial-Batch-Alignment
Use for large data sets that cannot be processed in a single batch using MS-Dial.  Will take excel export sheet and align features.

Name: Bryan Roberts
Date: 8/8/2019
Description: Takes different batches of excel sheets in the same folder as script from the same LC-MS run and combines 
features into a new excel sheet called "results.xlsx".  Features are aligned based on annotation name.  Steps for 
getting matching annotation names:
-process initial batch with ~200 samples and all MSMS samples
-reduce this data export and make mzrt from remaining ~3000 features
-mzrt name will be in the format name_adduct_mz_rt
-process remaining data in batches using new mz/rt and correcting retention times for each batch
-use python script to align data
Sources:
https://automatetheboringstuff.com/
http://prime.psc.riken.jp/Metabolomics_Software/MS-DIAL/
Excel File Format:
Standard exported output from MS-Dial
