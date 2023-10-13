<h1 align="center">Update Metadata for Delta Lake using Pydantic Data Models 📑</h1>
<p align="center">
    <img alt="Databricks" src="https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white" />
    <img alt="Delta" src="https://img.shields.io/badge/Delta-003366.svg?style=for-the-badge&logo=Delta&logoColor=white" />
    <img alt="Pydantic" src="https://img.shields.io/badge/Pydantic-E92063.svg?style=for-the-badge&logo=Pydantic&logoColor=white" />
</p>

## Introduction

This notebook is used to update metadata of an existing table in Delta Lake using the table's equivalent Pydantic data model. This is especially useful if you have data from an application that flows into Delta and happens to already have dataclasses or datamodels that define the schema of raw data.

> Note that updating Delta table metadata is highly dependent on the Pydantic models already being pre-defined with `tags` and `description` per `Field`

## Use Cases

The Delta Lake Table metadata updater is a helpful tool with below use cases:

1. **Metadata Enrichment**: Enhance the quality of your data by adding descriptions and tags to your table columns.

2. **Automated Documentation**: Save time and effort by automatically generating metadata based on your Pydantic data models.

3. **Consistency and Quality**: Ensure consistent metadata across your Delta Lake tables.

---
See more details in the notebook (ipynb or dbc)
