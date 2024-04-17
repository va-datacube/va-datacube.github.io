---
title: Configure AWS Access
layout: single
sidebar:
  nav: "docs"
toc: true
---
The VMASC VA Data Cube has access to many geospatial datasets hosted by different cloud providers such as Microsoft and AWS. In order to query and load datasets hosted in AWS, users must configure AWS credentials for the Data Cube package to utilize. 

Open Data Cube Products that require AWS acccess to be configured are:

- ls5_c2l2_st
- ls5_c2l2_sr
- ls7_c2l2_st
- ls7_c2l2_sr
- ls8_c2l2_st
- ls8_c2l2_sr
- ls9_c2l2_st
- ls9_c2l2_sr

## Configure AWS access in Jupyter Notebook

In order to configure AWS acccess, copy and paste the following lines of code before querying products :

```python
from datacube.utils.aws import configure_s3_access
configure_s3_access(profile='default', requester_pays=True)
```