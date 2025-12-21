# Data Extraction

This folder contains data extraction tables designed to support analysis of the research questions.

## Data Extraction Files

This folder contains the following Excel files:

### `RQ_Analysis_Strategy.xlsx`
This file contains the analysis strategy organized by research questions, including:
- Data extraction for RQ1 (RQ1a-RQ1e): Current approaches, tools, and models
  - Modality coverage (tables, charts, or both)
  - Task coverage (detection, structure recognition, data reconstruction, table-chart linking)
  - Model types (deep learning, rule-based, heuristic, hybrid, vision-language models)
- Data extraction for RQ2 (RQ2a): Multimodal alignment methods
  - Alignment mechanisms (text matching, embedding similarity, vision-language models)
  - Table-chart linking approaches
  - Shared metadata identification
  - Variable alignment across modalities

### `Comparison_Framework.xlsx`
This file contains the complete comparison framework with all annotated dimensions for the 68 included studies, including:
- **Full Data Extraction**: Article metadata (title, authors, year, source, DOI, peer-reviewed status, language)
- **Modality Coverage**: Tables, charts, or both
- **Task Coverage**: Specific extraction tasks addressed
- **Model Type**: Computational paradigm used
- **Dataset and Benchmark Use**: Public or proprietary datasets
- **Evaluation Metrics and Performance**: 
  - Metrics (precision, recall, F1-score, accuracy, IoU, numeric error)
  - Evaluation levels (component, structure, end-to-end)
  - Reported performance results
- **Artifact Availability**: Code, datasets, trained models, and demo availability
- **Level of Information Extracted**: Layout-level, label-level, value-level

## Data Format

All data extraction tables are provided in Excel format (.xlsx) for easy analysis and filtering.

## Data Availability

The complete annotation table resulting from the evaluation framework has been deposited on [Zenodo](https://zenodo.org/records/17590801).

## Related Documentation

- **Evaluation Framework**: See `evaluation_framework.md` in repository root
- **Paper Selection**: See `Paper Selection/` folder for selection process documentation
