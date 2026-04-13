# Ease with Data Databricks

This repository contains Databricks notebooks that demonstrate core lakehouse workflows in a development environment, including:

- Unity Catalog exploration and catalog creation
- Creating and populating Delta tables
- Running `MERGE` operations for upserts
- Deep vs. shallow clone examples
- Basic workspace and runtime checks

## Repository structure

- `project1/Catalog.ipynb` – Catalog inspection and catalog/external location creation examples.
- `project1/deep_shallow _clone.ipynb` – Table creation plus deep/shallow clone workflow snippets.
- `project1/merge.ipynb` and `project1/Delta merge.ipynb` – Delta merge/upsert examples using employee sample data.
- `project1/Write_emp_data.ipynb` and `project1/Run_write_emp.ipynb` – Employee data write/run workflow notebooks.
- `project1/NBW1.ipynb` – Basic notebook commands (`%sql`, `%sh`) and simple runtime checks.

## Prerequisites

To run these notebooks successfully, you should have:

1. Access to a Databricks workspace.
2. Permissions to create or query catalogs/schemas/tables in your target environment.
3. Access to referenced cloud storage paths and credentials (for external locations).

## How to use

1. Import this repository (or just the `project1/` folder) into Databricks Repos.
2. Attach each notebook to a cluster or SQL warehouse with appropriate permissions.
3. Execute cells from top to bottom.
4. Update hard-coded catalog names, schemas, storage URLs, and credential objects to match your environment before running DDL/DML statements.

## Notes

- These notebooks use development-oriented names such as `dev` and `dev.bronze`; adapt these for your own workspace conventions.
- Some notebooks are exploratory and may assume existing objects already exist.
- Review SQL cells before execution to avoid accidental changes in shared environments.
