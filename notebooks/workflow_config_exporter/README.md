# Databricks Workspace Job Configuration Exporter 🚀

## Introduction 📜

This notebook is used to fetch the workflow config from a workspace and then write it to disk thus helping one save a backup of their workflow config information.

## Use Cases 🌟

Areas where such a notebook may be helpful:

1. **Configuration Replication 🤝**

2. **Version Control 🔄**

3. **Disaster Recovery ☂️**

4. **Collaboration 🤗**

5. **Audit and Compliance 📊**

## Prerequisites 🛠️

To make the most of this notebook, it's important to ensure the following prerequisites are in place:

- Access to a Databricks workspace ([Access Token](https://docs.databricks.com/en/administration-guide/access-control/tokens.html)).
- Appropriate permissions for listing and viewing job configurations.

## Steps 📊

### 1. Fetch Job Configurations 📬

We fetch all the workflows present in your workspace, each fetched workflow config will also contain the individual task config present in the workflow and their respective job cluster configs. [Databricks API documentation](https://docs.databricks.com/api/workspace/jobs/list).  

### 2. Parse Information 🧩

In this step we parse the obtained config info. The main thing to keep in mind is that the cluster config contains some fields which are populated after the cluster is initialized but will be fetched anyway from step 1, we need to remove this field or else when we use the same config to create the workflow later it will throw an error. You can also add any custom logic here. For example: You can include webhook notification ID to be associated with a workflow you like, You can also associate an existing all-purpose-compute to a workflow that you want, etc.  

### 3. Save Configuration to JSON 💾

We later save the config to file, if you have a mounted s3 bucket or an azure data lake storage you can direcly specify the path as dbutils will take care of the rest. If you are running the notebook locally then you will need to change the code and use python's inbuilt `open` function to get the task done.

--- 
