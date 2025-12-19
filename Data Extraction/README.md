# Data Extraction

This folder contains data extraction tables designed to support analysis of the research questions.

## Data Extraction Tables

### Full Data Extraction
Complete dataset including article metadata:
- Title
- Authors
- Publication year
- Source database
- DOI
- Peer-reviewed status
- Language

### Data Extraction for RQ1 (RQ1a-RQ1e)
Information related to current approaches, tools, and models:
- **Modality Coverage**: Tables, charts, or both
- **Task Coverage**: 
  - Table detection
  - Table structure recognition
  - Chart detection
  - Chart component detection
  - Data reconstruction
  - Table-chart linking
- **Model Type**: 
  - Deep learning (CNNs, Transformers)
  - Rule-based
  - Heuristic
  - Hybrid
  - Vision-language models

### Data Extraction for RQ2 (RQ2a)
Information on multimodal alignment:
- Alignment mechanisms (text matching, embedding similarity, vision-language models)
- Table-chart linking approaches
- Shared metadata identification
- Variable alignment across modalities

### Evaluation Metrics and Performance
Evaluation practices across studies:
- **Metrics**: Precision, recall, F1-score, accuracy, IoU, numeric error
- **Evaluation Levels**: 
  - Component level
  - Structure level
  - End-to-end system level
- **Reported Performance**: Quantitative results when available

### Artifact Availability
Documentation of publicly available resources:
- Code availability
- Dataset availability
- Trained model availability
- Demo availability

## Data Format

Data extraction tables are provided in Excel format (.xlsx) for easy analysis and filtering.

## Data Availability

The complete annotation table resulting from the evaluation framework has been deposited on [Zenodo](https://zenodo.org/records/17590801).

## Related Documentation

- **Evaluation Framework**: See `evaluation_framework.md` in repository root
- **Paper Selection**: See `Paper Selection/` folder for selection process documentation
