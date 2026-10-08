# VulFileHunter: Leveraging Description Augmentation with Large Language Models for Vulnerability-Relevant File Uncovery

## Framework
![](./framework.png)

## Code

### CVE Analyst
The CVE Analyst module first enhances the original CVE descriptions by collecting supplementary information from external references and online sources, addressing gaps and incomplete details.

### Repo Explorer
The Repo Explorer module identifies relevant open-source repositories and filters candidate files based on the augmented CVE descriptions, effectively narrowing the scope for localizing vulnerability-relevant files.

### VulHunter
The Vul Hunter module performs precise localization by analyzing file hierarchies and conducting LLM-based semantic analysis to identify vulnerability-relevant files.

## Dataset
- **dataset.json**: The dataset contains 1729 CVEs in total, and each record includes repository, commits, and vulnerability_files.
- **cve_metadata**: full data can be downloaded from https://nvd.nist.gov/vuln/data-feeds#JSON_FEED

## Result
![](./Result/Overall_Performance.png)
![](./Result/RQ2_Accuracy.png)
![](./Result/RQ2_Completeness.png)
![](./Result/RQ3.png)
![](./Result/Ablation_Study.png)
![](./Result/RQ5.png)