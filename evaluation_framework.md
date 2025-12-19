# Evaluation Framework Documentation

This document describes the evaluation framework used to analyze the 68 included studies in the systematic literature review on table and chart extraction from scientific publications.

## Framework Dimensions

Each publication was analyzed according to the following characteristics, aligned with the research questions defined in the methodology:

### 1. Modality Coverage

**Description:** Identifies whether the approach targets tables, charts, or both.

**Values:**
- `Tables` - Only table extraction
- `Charts` - Only chart extraction
- `Both` - Both tables and charts

**Research Question Alignment:** RQ1a (existing approaches and tools), RQ2a (integration across modalities)

### 2. Task Coverage

**Description:** Specifies which extraction tasks are addressed by the system.

**Possible Tasks:**
- Table detection
- Table structure recognition
- Table cell extraction
- Chart detection
- Chart component detection (bars, lines, points, etc.)
- Axis and legend extraction
- Data reconstruction (chart-to-table conversion)
- Table-chart linking/alignment
- Variable identification
- Metadata extraction

**Research Question Alignment:** RQ1a-RQ1e (extraction tasks and pipelines)

### 3. Model Type

**Description:** Describes the computational paradigm used.

**Values:**
- `Deep Learning` - CNNs, Transformers, or other deep learning architectures
- `Rule-based` - Systems relying on explicitly defined rules or patterns
- `Heuristic` - Simplified, task-specific decision strategies
- `Hybrid` - Combination of rule-based and learning-based approaches
- `Vision-Language Models` - Models that integrate visual and textual information

**Research Question Alignment:** RQ1b (model architectures), RQ1d (chart extraction models)

### 4. Dataset and Benchmark Use

**Description:** Specifies whether public or proprietary datasets are used and the presence of benchmark standardization.

**Values:**
- `Public Dataset` - Uses publicly available datasets
- `Proprietary Dataset` - Uses private or custom datasets
- `Both` - Uses both public and proprietary datasets
- `Not Specified` - Dataset information not clearly stated

**Common Datasets:**
- Table datasets: PubTables, TableBank, ICDAR, etc.
- Chart datasets: ChartQA, PlotQA, Chart-to-Text, etc.

**Research Question Alignment:** RQ1b (reproducibility), RQ1c (evaluation resources)

### 5. Evaluation Metrics and Reported Performance

**Description:** Records the evaluation metrics explicitly reported and the level at which performance is assessed.

**Common Metrics:**
- Precision
- Recall
- F₁-score
- Accuracy
- Intersection-over-Union (IoU)
- Numeric error or deviation
- Task-specific measures (cell-level accuracy, axis parsing accuracy, value reconstruction error)

**Evaluation Levels:**
- Component level (e.g., table detection, header identification, chart element detection)
- Structure level (e.g., row/column reconstruction, chart-to-table conversion)
- End-to-end system level

**Research Question Alignment:** All RQs (performance assessment and comparability)

### 6. Availability of Artifacts

**Description:** Indicates whether code, datasets, trained models, or demos are publicly available.

**Values:**
- `Code Available` - Source code is publicly available
- `Dataset Available` - Dataset is publicly available
- `Model Available` - Trained models are publicly available
- `Demo Available` - Online demo or interface is available
- `Not Available` - Artifacts are not publicly available
- `Not Specified` - Availability not clearly stated

**Research Question Alignment:** RQ1a (practical reproducibility and transparency)

### 7. Level of Information Extracted

**Description:** Describes the level at which information is extracted.

**Levels:**
- **Layout-level extraction:** Detection of rows, columns, cells, or chart components
- **Label-level extraction:** Headers, axis titles, legends, units
- **Value-level association:** Explicit linking of labels or variables to numerical values

**Research Question Alignment:** RQ1f (variable identification), RQ2a (information alignment)

## Annotation Process

1. **Manual Annotation:** Each paper was manually annotated across all dimensions using information from:
   - The publication itself
   - Supplementary materials
   - Associated open-source repositories (when available)
   - Demo pages (when available)

2. **Missing Information:** When a criterion was not explicitly reported, it was marked as "Not Specified."

3. **Consistency:** Manual curation ensured consistency and traceability across all 68 papers.

## Data Availability

The complete annotation table resulting from the evaluation framework has been deposited on Zenodo: https://zenodo.org/records/17590801

The deposit includes:
- Full spreadsheet with all annotated characteristics
- Screening decisions for each paper
- Documentation of the annotation process

## Usage

This framework enables:
- Systematic comparison of technical scope across studies
- Analysis of modeling choices and trends
- Assessment of dataset usage and evaluation practices
- Identification of gaps in current research
- Evaluation of reproducibility and transparency

## Research Question Mapping

| Framework Dimension | Research Questions |
|---------------------|---------------------|
| Modality Coverage | RQ1a, RQ2a |
| Task Coverage | RQ1a-RQ1e |
| Model Type | RQ1b, RQ1d |
| Dataset and Benchmark Use | RQ1b, RQ1c |
| Evaluation Metrics | All RQs |
| Availability of Artifacts | RQ1a |
| Level of Information Extracted | RQ1f, RQ2a |

