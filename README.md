<h1 align="center">Databricks Helpers 🧱</h1>

<p align="center">
    <img alt="Databricks" src="https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white" />
    <img alt="Delta" src="https://img.shields.io/badge/Delta-003366.svg?style=for-the-badge&logo=Delta&logoColor=white" />
    <br><br>
    <img alt="Plotly" src="https://img.shields.io/badge/Plotly-3F4F75.svg?style=for-the-badge&logo=Plotly&logoColor=white" />
    <img alt="Pydantic" src="https://img.shields.io/badge/Pydantic-E92063.svg?style=for-the-badge&logo=Pydantic&logoColor=white" />
</p>

<p align="center">
    Easy-to-use Databricks Notebooks for Admin Tasks.
    <br>Made with ❤️ by <a href="https://www.dotlas.com">Dotlas Inc</a>
</p>

## About

This repository contains a directory of Databricks notebooks that assists with administrative tasks for Databricks, or otherwise helps as a supporting utility.

For example, consider the following use-cases:

* 📆 View a calendar of scheduled jobs to resolve conflicts in Databricks workflows.
* 🐼 Upload a [Pandas](https://pypi.org/project/pandas) DataFrame to Delta Lake
* 📑 Update Delta Lake table Documentation using [Pydantic](https://docs.pydantic.dev/latest/) Models
* ➿ Migrate Jobs between Databricks workspaces
* ⚙️ Mass-edit Job Clusters in Existing Jobs

## Directory

| Notebook | Description |
| --- | --- |
| [Workflow Calendar](./notebooks/workflow_calendar/README.md) | Visualize scheduled Jobs on a calendar, eyeball conflicts and view historic runs as a [Gantt](https://en.wikipedia.org/wiki/Gantt_chart) chart |
| [Delta Docs with Pydantic](./notebooks/delta_docs_pydantic/README.md) | If you have pydantic models with fields containing `description` and `tags` that are used as data models, transfer these field descriptions to Delta lake columns as comments and tags. |
| [Pandas to Delta](./notebooks/pandas_delta/README.md) | Use [databricks-sql-python](https://github.com/databricks/databricks-sql-python/) and [SQLAlchemy](https://pypi.org/project/sqlalchemy/) to upload a Pandas DataFrame to Delta Lake from outside a Databricks environment |
| [Workspace Jobs Migration](./notebooks/migrate_workspace/README.md) | Migrate Workflows from one Databricks workspace to another |
| [Job Cluster Update](./notebooks/update_job_cluster/README.md) | Use the Databricks API to mass-update Job and Task configs |
| [Workflow Config Exporter](./notebooks/workflow_config_exporter/README.md) | Export existing workflow configuration and save it for future consumption |
