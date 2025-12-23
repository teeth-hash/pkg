# pkg
pkg dataset
# Patent Knowledge Graph Construction

This repository describes the construction process of the **Patent Knowledge Graph (PKG)** used in this study.

## Overview

The PKG is built through a **three-stage pipeline** that transforms raw patent data into a structured and semantically enriched knowledge graph.

## Pipeline

### 1. Patent Data Collection and Preprocessing
- Data source: **Google Patents**（https://ggp.purplevineip.com/）
- Large-scale patent metadata collection
- Data cleaning, normalization, and deduplication
- Extraction of structured entities:
  - Patent
  - Inventor
  - Organization

### 2. Semantic Entity and Relation Extraction
- Target semantic entities:
  - Technical Field
  - Technical Topic
- Task-oriented prompt templates are designed
- **ChatGPT API** is used to extract entities and relations from unstructured patent texts
- Results are manually validated to ensure semantic accuracy and consistency

### 3. Knowledge Graph Integration
- Entities and relations are integrated following a predefined **Patent Knowledge Graph schema**
- Entity alignment and relation normalization
- Final PKG construction

## Output
- A complete and scalable Patent Knowledge Graph
- Supports graph-based analysis and learning tasks
