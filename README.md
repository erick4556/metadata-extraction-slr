# Table-Chart-Extraction-SLR

Extracting structured data from tables and charts in scientific publications remains a critical challenge for automated knowledge extraction and meta-analysis. This project presents a **Systematic Literature Review (SLR)** focused on methods, models, and pipelines for table and chart extraction from scientific documents. We analyzed 68 peer-reviewed papers and extracted information across multiple dimensions including modality coverage, task types, model architectures, evaluation practices, and application domains.

---

## Repository Structure

### `Paper Selection/`

This folder documents the **paper selection process**, with each filtering step tracked for full transparency and reproducibility. The folder contains the following Excel files:

* `Raw_Search.xlsx` - Initial retrieval of 8,398 records from all databases
* `Deduplicated_Records.xlsx` - Records after duplicate removal (7,678 unique entries)
* `Title_Screening.xlsx` - Records after title screening (565 studies)
* `Abstract_Screening.xlsx` - Records after abstract screening (68 studies)

The screening process includes the following steps:

1. **Initial Retrieval**  
   Search queries were executed across six major academic databases and search engines:
   - Web of Science
   - Scopus
   - IEEE Xplore
   - ACM Digital Library
   - SpringerLink
   - Publish or Perish (Google Scholar, Semantic Scholar, Lens.org, Crossref)
   
   The following search query templates were used (adapted to each database's syntax):
   - `"table extraction" AND "chart extraction"`
   - `"chart understanding" AND "table understanding"`
   - `"figure extraction" OR "table extraction"`
   - `"multimodal" AND ("scientific publications" OR "scientific articles") AND ("tables" OR "charts")`
   - `"chart data reconstruction" AND "scientific publications"`
   
   The combined retrieval yielded **8,398 records** based on these keyword queries.

2. **Duplicate Removal**  
   Deduplication across databases using multiple strategies (DOI matching, fingerprint matching, title similarity) reduced the dataset to **7,678 unique entries**.

3. **Title Screening**  
   Title screening was performed based on inclusion keywords, narrowing the pool to **565 potentially relevant papers**.

4. **Abstract Screening**  
   We applied abstract-based screening using inclusion/exclusion criteria, resulting in **68 papers**.

5. **Full-text Evaluation**  
   Final application of formal inclusion criteria (IC1-IC4) and exclusion criteria (EC1-EC4) to the 68 papers, resulting in **68 final included studies**.

These 68 papers form the core dataset for downstream analysis. From them, we extracted information across seven evaluation framework dimensions, addressing research questions on extraction approaches, model architectures, data transformation pipelines, chart understanding, variable identification, and multimodal alignment.

---

### `Data Extraction/`

This folder includes data extraction tables designed to support analysis of our research questions (RQs). The folder contains the following Excel files:

* `RQ_Analysis_Strategy.xlsx` - Analysis strategy organized by research questions
* `Comparison_Framework.xlsx` - Complete comparison framework with all annotated dimensions for the 68 included studies

* **Full Data Extraction**  
  Dataset including article metadata such as title, authors, year, source database, DOI, and peer-reviewed status.

* **Data Extraction for RQ1**  
  Used to analyze **RQ1a-RQ1e** (Current approaches, tools, and models for data extraction from tables and charts).  
  Includes modality coverage (tables, charts, or both), task coverage (detection, structure recognition, data reconstruction), and model types.

* **Data Extraction for RQ2**  
  Used to analyze **RQ2a** (Methods for identifying and aligning related information across tables and charts).  
  Contains information on multimodal alignment mechanisms, table-chart linking approaches, and shared metadata identification.

* **Evaluation Metrics and Performance**  
  Used to analyze evaluation practices across studies.  
  Includes evaluation metrics (precision, recall, F1-score, accuracy, IoU), evaluation levels (component, structure, end-to-end), and reported performance results.

* **Artifact Availability**  
  Documents the availability of code, datasets, trained models, and demos for each included study.

---

### `evaluation_framework.md`

This document (located in the repository root) describes the complete evaluation framework used to analyze the 68 included studies. The framework organizes information across seven dimensions:

1. **Modality Coverage** - Tables, charts, or both
2. **Task Coverage** - Specific extraction tasks addressed
3. **Model Type** - Computational paradigm (deep learning, rule-based, hybrid, etc.)
4. **Dataset and Benchmark Use** - Public or proprietary datasets
5. **Evaluation Metrics and Reported Performance** - Metrics used and performance levels
6. **Availability of Artifacts** - Code, datasets, models availability
7. **Level of Information Extracted** - Layout-level, label-level, value-level

Each dimension is aligned with specific research questions and includes detailed documentation of possible values and annotation guidelines.

---

## Research Questions

This systematic review addresses the following research questions:

**RQ1a:** What are the current approaches, tools, and models for data extraction from tables and charts in scientific publications?

**RQ1b:** What models and architectures (e.g., CNNs, Transformers, hybrid systems) are used for tabular data extraction?

**RQ1c:** How do existing systems transform tables from unstructured document formats (e.g., PDFs) into machine-readable representations?

**RQ1d:** What tools and models are used to extract data from charts?

**RQ1e:** How do current methods reconstruct the underlying data represented in charts into structured tabular formats?

**RQ1f:** How do existing methods identify and interpret variables within tables and charts?

**RQ2a:** How do current methods identify and align related information across tables and charts within the same scientific publication?

---

## Data Availability

* **Annotation data**: Available on [Zenodo](https://zenodo.org/records/17590801)
* **Raw search results**: Available upon request (subject to database licensing agreements)
* **Processed data**: Available in `Paper Selection/` and `Data Extraction/` folders
* **Evaluation framework**: Complete documentation available in `evaluation_framework.md`


## Acknowledgments

This systematic review follows the methodology established by Kitchenham and Charters (2007) for conducting systematic literature reviews, ensuring transparency, reproducibility, and consistency throughout the process.
