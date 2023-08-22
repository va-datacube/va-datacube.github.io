---
title: Install Python Packages
layout: single
sidebar:
  nav: "docs"
toc: true
---

# Creating a Conda Data Cube Environment 

This guide will walk you through the process of creating a new Conda environment for Data Cube analysis that requires additonal python packages not installed on the VMASC VA Data Cube.

## Step 1: Open Jupyter Terminal

1. Navigate to [VMASC VA Open Data Cube](https://datacube.online).
2. Once open, from the **Launcher**, select **Terminal** to open a new terminal window within the Data Cube.

## Step 2: Create a Conda Environment

In the Terminal, you will now create a new Conda environment based on the existing base environment.

1. To create a new Conda environment based on the Data Cube base environment, use the following command:

    ```bash
   conda create --name myenv --clone base
    ```

After executing, the command will take a minute or two to clone, download, and extract all packages from the base enviornment for your newly created one. 

> You will be notified two packages that could not be cloned, mamba and conda which are not needed for Data Cube anaylysis.

## Step 3: Activate the New Environment

1. Once the environment is created, you need to activate it. Use the following command:

    ```bash
    conda activate myenv
    ```

2. After activation, your terminal prompt should change to indicate that you are now working within the myenv environment.

## Step 4: Install Additional Packages

With your new Conda environment activated, you can install additional packages that are specific to your needs. For example:

```bash
conda install numpy pandas matplotlib
```

## Step 6: Deactivating the Environment

When you're done working in your Conda environment, you can deactivate it to return to the base environment:

```bash
conda deactivate
```

# Resources

- [Conda.io](https://conda.io)
- [Conda Command reference](https://docs.conda.io/projects/conda/en/stable/commands/index.html)