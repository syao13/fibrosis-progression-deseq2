# The fibrosis progression study

## Introduction
This repo aims to run the analysis following the paper [Hepatic expression profiling identifies steatosis-independent and steatosis- driven advanced fibrosis genes](https://insight.jci.org/articles/view/120274). In the paper, the authors performed RNA sequencing on liver biopsies of patients with different fibrosis stages, from both infection with hepatitis C virus (HCV) or non-alcholic fatty liver disease patients. For simplicity and specificity, I will mainly focus on fatty liver disease. Therefore, the main goal of this analysis is the follwoing:  

* Compare results with what's in the paper and check if the fibrosis progression is significantly different between fatty liver disease patients only (this repo) and both HCV and fatty liver disease patients (the paper).
* Check if the analysis can be purely run in Python, as Python has been gaining it popularity in the bioinformatics field. The paper uses mainly R packages.
* Check if updates in functional databases, such as KEGG or GO, would results in any new findings in enrichment analysis.

Also as a stretch goal, the following will also be checked:
* FDA has recently (March 14, 2024) approved the first ever treatment of adults with noncirrhotic non-alcoholic steatohepatitis (NASH) with moderate to advanced liver scarring (fibrosis), to be used along with diet and exercise: Rezdiffra. Rezdiffra is a partial agonist of THR‑β, which is the major form of THR in the liver, and stimulation of THR‑β in the liver reduces intrahepatic triglycerides. Therefore, I'd like to check if any of the THR‑β related pathways is signaled from the data.
* Check if the result of the study can provide other insights in any other potential drug target.

## Dataset
The raw and processed data from the paper is available at ArrayExpress (https://www.ebi.ac.uk/arrayexpress/) under accession E-MTAB-6863. Download the datasets to the datasets folder to run the analysi.

## Project Setup
  * First Clone the repository.
  * Create the virtual environment for the project. 
  ```sh
  $ conda create -n myenv python=3.10
  ```
  * Install the required packages using requirements.txt inside the environemnt using pip.
  ```sh
  $ pip install -r requirements.txt
  ```
  * run the notebooks in order.
