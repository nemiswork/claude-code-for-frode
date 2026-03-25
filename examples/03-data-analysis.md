# Example 3: Data Analysis

> Time: ~15 minutes
> Goal: Analyze a proteomics dataset, create visualizations, write analysis scripts

## The Sample Dataset

This repo includes `sample-data/proteomics-sample.csv` — a simulated TMT proteomics dataset with protein expression across Alzheimer's and control CSF samples. Let's put Claude to work on it.

## Basic Exploration

### Understand the Data

```
Read sample-data/proteomics-sample.csv and tell me:
1. How many proteins and samples?
2. What are the experimental groups?
3. Data quality — any missing values, outliers, or concerns?
4. Summary statistics per group
```

### Quick Visualization

```
Create a Python script that reads the proteomics dataset and generates:
1. A box plot comparing protein expression distributions across all samples
2. A PCA plot colored by group (Alzheimer's vs Control)
3. A correlation heatmap of all samples

Save the plots as PNG files and show them to me.
```

## Statistical Analysis

### Differential Expression

```
Perform a differential expression analysis on the proteomics dataset:
- Compare Alzheimer's vs Control
- Use a t-test with Benjamini-Hochberg correction
- Calculate log2 fold changes
- Create a volcano plot highlighting significant proteins (adj. p < 0.05, |log2FC| > 1)
- Save the results table as significant-proteins.csv
```

### Pathway Analysis

```
Take the significant proteins from the previous analysis and:
1. Look up their gene names
2. Search for enriched biological pathways using GO terms
3. Present the top 10 enriched pathways
4. Create a bar chart of the enrichment results
```

## Working With Your Own Data

When you have real data to analyze, just point Claude at it:

```
Read /Users/frode/Downloads/my-experiment-results.csv and analyze it
the same way we did with the sample data. Adjust the analysis based on
what you find — I trust your judgment on the right statistical approach.
```

### Excel Files Work Too

```
Read /Users/frode/Desktop/patient-cohort-data.xlsx and summarize it.
Focus on the demographics and any correlations with protein expression levels.
```

### Large Datasets

For bigger files, Claude can write scripts that process them efficiently:

```
I have a MaxQuant proteinGroups.txt file (150MB) in my Downloads folder.
Write a Python script that:
1. Loads only the relevant columns (protein IDs, gene names, LFQ intensities)
2. Filters out reverse hits and contaminants
3. Log2 transforms the intensities
4. Exports a clean CSV ready for downstream analysis
```

## Automation

### Reusable Analysis Pipeline

```
Create a Python script called analyze_proteomics.py that I can reuse:
- Takes a CSV file path as input
- Automatically detects groups from column names
- Runs differential expression
- Generates volcano plot, PCA, and heatmap
- Saves everything to an 'output' folder
- Include clear comments so I understand each step

I want to be able to run it like: python analyze_proteomics.py my-data.csv
```

## What You Just Learned

- Claude handles real data analysis workflows
- It writes and runs Python scripts for you
- It generates publication-quality figures
- It understands proteomics-specific workflows (TMT, LFQ, MaxQuant)
- You can build reusable tools without writing code yourself

> *The data doesn't lie, Frode. Unlike... well, you know what you think about Big Pharma's clinical trial data. But let's not go there.*

**Next:** [04-writing-partner.md](04-writing-partner.md) — Claude as your writing assistant.
