---
title: Jupyter AI
layout: single
sidebar:
  nav: "docs"
toc: true
---

Thanks to the wonderful team at Project Jupyter, AI chat models are now accessible from within Jupyter Notebooks. This capability has been made available within VMASC VA Data Cube Jupyter Notebooks with the [jupyter-ai-magics](https://pypi.org/project/jupyter-ai-magics/) package and is relatively new so if you run into any issues please don't hesitate to contact the Data Cube team at **Datacube@odu.edu**.


## Jupyter AI Magic - Model Providers

Jupyter AI supports a wide range of model providers and models. To use Jupyter AI with a particular provider, you must install its Python packages and set its API key (or other credentials) in your environment. 

Jupyter AI supports the following model providers:

| Provider            | Provider ID          | Environment variable       | Python package(s)               |
|---------------------|----------------------|----------------------------|---------------------------------|
| AI21                | `ai21`               | `AI21_API_KEY`             | `ai21`                          |
| Anthropic           | `anthropic`          | `ANTHROPIC_API_KEY`        | `anthropic`                     |
| Bedrock             | `amazon-bedrock`     | N/A                        | `boto3`                         |
| Cohere              | `cohere`             | `COHERE_API_KEY`           | `cohere`                        |
| Hugging Face Hub    | `huggingface_hub`    | `HUGGINGFACEHUB_API_TOKEN` | `huggingface_hub`, `ipywidgets`, `pillow` |
| OpenAI              | `openai`             | `OPENAI_API_KEY`           | `openai`                        |
| OpenAI (chat)       | `openai-chat`        | `OPENAI_API_KEY`           | `openai`                        |
| SageMaker           | `sagemaker-endpoint` | N/A                        | `boto3`                         |




### Jupyter AI Magic - Set up Model Providors in Notebook


To use any AI model provider within notebooks, you'll need the appropriate credentials, such as API keys.

Obtain the necessary credentials (e.g., API keys) from your model provider's platform.

You can set your keys using environment variables or in a code cell in your notebook.
In a code cell, you can use the %env magic command to set the credentials as follows:

```python
# NOTE: Replace 'PROVIDER_API_KEY' with the credential key's name,
# and replace 'YOUR_API_KEY_HERE' with the key.
%env PROVIDER_API_KEY=YOUR_API_KEY_HERE
```
## Jupyter AI Magic Command Usage

To use the AI magic command, follow the [user guide](https://jupyter-ai.readthedocs.io/en/latest/users/index.html#the-ai-and-ai-magic-commands) and [examples](https://github.com/jupyterlab/jupyter-ai/tree/main/examples) created by the Project Jupyter Team.
