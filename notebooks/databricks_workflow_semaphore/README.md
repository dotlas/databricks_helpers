<h1 align="center">Databricks Workflow Pause/Unpause Utility ⏸️▶️</h1>
<p align="center">
    <img alt="Databricks" src="https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white" />
</p>

## Introduction

This notebook enables safe and efficient pausing or unpausing of scheduled Databricks jobs based on a user-defined keyword. It is ideal for operational testing, deployment workflows, and temporary job management.

## Use Cases

This notebook is helpful for:

1. **Operational Testing**: Unpause workflows for testing in controlled environments.
2. **Scheduled Job Auditing**: Quickly identify and control active scheduled jobs via keyword filtering.
3. **Temporary Suppression**: Suppress scheduled job execution during holidays or system maintenance.
4. **Bulk Control**: Apply pause/unpause actions across many jobs with a single keyword-driven command.

## Parameters

| Name        | Description                                | Default | Allowed Values      |
|-------------|--------------------------------------------|---------|---------------------|
| `KEYWORD`   | Required string to match in job names       | (empty) | Any string          |
| `OPERATION` | Action to apply to matching jobs            | PAUSE   | `PAUSE`, `UNPAUSE`  |
