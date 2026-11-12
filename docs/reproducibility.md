# Reproducibility

## Environment

The original work ran on an institution-managed Spark cluster with data stored in Azure Blob Storage through HDFS-compatible `wasbs://` paths. A public user will need to provide their own data locations and Spark configuration.

## Public notebooks

Public notebook versions should:

1. contain no access tokens, SAS values, usernames, private storage paths, or institutional hostnames;
2. define all configurable paths in one clearly labelled setup cell;
3. separate data loading, validation, transformation, modelling, evaluation, and visualization;
4. use deterministic seeds or hash-based splits where possible;
5. avoid committing generated outputs, checkpoints, or raw data;
6. include a small-data or sample-data mode when licensing permits;
7. state which stages require a distributed Spark environment.

## Data

Raw datasets are not distributed through this repository. Users should obtain the relevant public datasets from their official providers and follow their licensing and usage requirements.

## Expected differences

Exact performance and counts can change if a public reproduction uses a different archive date, source mirror, Spark version, partition layout, or random seed. The case-study documentation therefore emphasizes the validated workflow and the results from the original execution environment.

