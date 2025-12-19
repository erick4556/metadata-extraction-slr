# Paper Selection Process

This folder documents the complete paper selection process for the systematic literature review.

## Selection Workflow

The paper selection process was conducted in five sequential phases:

### 1. Initial Retrieval
- **Total records retrieved**: 8,398
- **Sources**: Web of Science, Scopus, IEEE Xplore, ACM Digital Library, SpringerLink, Publish or Perish
- **Search queries**: The following 5 query templates were used (adapted to each database's syntax):
  - `"table extraction" AND "chart extraction"`
  - `"chart understanding" AND "table understanding"`
  - `"figure extraction" OR "table extraction"`
  - `"multimodal" AND ("scientific publications" OR "scientific articles") AND ("tables" OR "charts")`
  - `"chart data reconstruction" AND "scientific publications"`
  
  For Publish or Perish (which accesses Google Scholar, Semantic Scholar, Lens.org, and Crossref), these queries were executed with simplified syntax suitable for keyword-based search engines.
- **Date range**: All publications up to April 1, 2025

### 2. Duplicate Removal
- **Records after deduplication**: 7,678
- **Duplicates removed**: 720
- **Deduplication strategies**:
  - Exact match on DOI (when available)
  - Exact match on fingerprint (title + authors + year)
  - High similarity on normalized title (>95%)

### 3. Title Screening
- **Records after title screening**: 565
- **Excluded**: 7,113
- **Screening method**: Keyword-based screening using inclusion keywords

### 4. Abstract Screening
- **Records after abstract screening**: 68
- **Excluded**: 497
- **Screening method**: Abstract-based screening using inclusion/exclusion criteria

### 5. Full-text Evaluation
- **Final included studies**: 68
- **Excluded**: 0 (all 68 met the inclusion criteria)
- **Evaluation method**: Formal application of inclusion criteria (IC1-IC4) and exclusion criteria (EC1-EC4)

## Documentation

The selection process is documented in:
- Screening decisions recorded in annotation sheets
- Deduplication summary statistics
- Screening phase summaries

## Transparency

All screening decisions were recorded to ensure transparency and reproducibility. The complete annotation framework and screening decisions are available on [Zenodo](https://zenodo.org/records/17590801).
