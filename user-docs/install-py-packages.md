---
title: Install Python Package(s)
layout: single
sidebar:
  nav: "docs"
toc: true
---

The VMASC VA Data Cube environment contains many geospatial python packages required for analysis but there may be some you need that we don't have. If there is a package you need, simply launch a terminal within the Data Cube and install any package using pip. 

## Step 1: Open Jupyter Terminal

1. Navigate to [VMASC VA Open Data Cube](https://datacube.online).
2. Once open, from the **Launcher**, select **Terminal** to open a new terminal window within the Data Cube.

![image-center]({{ site.url }}{{ site.baseurl }}/images/launch-terminal.png){: .align-center}

## Step 2: Install Python Package(s)

With the terminal launched, install python package(s).

```bash
pip install numpy
```
> The package(s) installed will be local to your user on the Data Cube and not accessible by others.


