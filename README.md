# The Fibrosis Progression Study

## Introduction
This repo aims to run the analysis following the paper [Hepatic expression profiling identifies steatosis-independent and steatosis- driven advanced fibrosis genes](https://insight.jci.org/articles/view/120274). In this paper, the authors performed RNA sequencing on liver biopsies of patients with different fibrosis stages, from both infection with hepatitis C virus (HCV) or non-alcholic fatty liver disease (NAFLD) patients. For the purpose of this analysis, the focus will be primarily on NAFLD. The main objectives of this analysis are:

  * **Evaluate the feasibility of conducting the analysis exclusively in Python**: The original paper predominantly utilizes R packages. Given Python's increasing popularity in data analytics and production pipelines as well as in the bioinformatics field, this analysis will explore the viability of using Python exclusively.
  * **Investigate the impact of updated functional databases**: Examine if new updates in databases such as KEGG or GO, compared to the pre-2018 versions used in the paper, yield new insights in the enrichment analysis.
  * **Compare the fatty liver results with the findings of the original paper**: Assess whether fibrosis progression is significantly different when considering only NAFLD patients (this analysis) versus both HCV and NAFLD patients (the original paper).


Additionally, the following stretch goals will be investigated:

   * **Examine the influence of recent FDA-approved treatments**: On March 14, 2024, the FDA approved Rezdiffra, the first treatment for noncirrhotic non-alcoholic steatohepatitis (NASH) with moderate to advanced liver scarring (fibrosis). Rezdiffra is a partial agonist of THR-β, which is the predominant form of THR in the liver, and stimulation of THR-β in the liver reduces intrahepatic triglycerides. This analysis will explore if any THR-β related pathways are signaled in the data.
   * **Identify potential new drug targets**: Evaluate if the results of this study provide insights into other potential drug targets for fibrosis progression in NAFLD patients.

## Dataset
The raw and processed data from the paper is available at [ArrayExpress](https://www.ebi.ac.uk/arrayexpress/) under accession number E-MTAB-6863. Download the datasets to the `datasets` folder to run the analysis.

## Project Setup
  * First Clone the repository.
  * Create the virtual environment for the project. 
  ```sh
  $ conda create -n myenv python=3.10
  $ conda activate myenv
  ```
  * Install the required packages using requirements.txt inside the environemnt using pip.
  ```sh
  $ pip install -r requirements.txt
  ```
  * Run the notebooks in order.
