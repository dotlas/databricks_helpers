<h1 align="center">Automated Staleness Monitoring for Delta Lake Tables 🕵️</h1>
<p align="center">
    <img alt="Databricks" src="https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white" />
    <img alt="Delta" src="https://img.shields.io/badge/Delta-003366.svg?style=for-the-badge&logo=Delta&logoColor=white" />
    <img alt="Slack" src="https://img.shields.io/badge/Slack-4A154B.svg?style=for-the-badge&logo=Slack&logoColor=white" />
</p>

## Introduction

This notebook provides an automated solution for monitoring and managing stale Delta Lake tables within a Databricks Unity Catalog environment. It systematically analyzes table history to identify assets that haven't had recent data-changing operations, helping to maintain a clean and cost-effective data lake.

> This notebook is designed as a configurable utility. Before execution, users must define their own rules for staleness thresholds, table exclusion policies, and notification settings to tailor the tool to their specific environment.

## Use Cases

The Delta Lake Staleness Monitor is a helpful tool with the below use cases:

1.  **Cost Optimization**: Reduce cloud storage costs by automatically identifying and cleaning up unused or abandoned Delta tables.

2.  **Improved Data Governance**: Maintain a high-quality data environment by flagging stale assets that may contain outdated or irrelevant information.

3.  **Automated Housekeeping**: Save significant manual effort by creating a scheduled workflow that automatically detects and manages stale tables across your workspace.

4.  **Proactive Team Alerts**: Keep data teams informed by sending automatic Slack notifications about tables that require review, enabling them to take action before data becomes obsolete.

---
See more details in the notebook (ipynb)