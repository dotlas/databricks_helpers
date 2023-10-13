<h1 align="center">Workspace Migration ✈️</h1>
<p align="center">
    <img alt="Databricks" src="https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white" />
</p>

## Introduction

This notebook is used to migrate clusters and workflows from one workspace to another using the Databricks REST API. It works by fetching the current cluster / workflow configs and then using it to create the same in a new workspace.

## Use Cases

Areas where such a notebook may be helpful:

1. **Migrating clusters and workflows to a new workspace**: This is the obvious use case, and the notebook would be particularly useful for large or complex workspaces, where migrating everything manually would be time-consuming and error-prone.
2. **Creating a new workspace from scratch**: The notebook could be used to quickly create a new workspace with the same clusters and workflows as an existing workspace. This could be useful for creating a development or staging environment, or for creating a new workspace for a specific project or team.

---
See more details in the notebook (ipynb)
