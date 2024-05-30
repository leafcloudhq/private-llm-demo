# Private LLM Using Ollama and Anything llm

This repository contains the necessary files and instructions to set up a private large language model (LLM) environment using Kubernetes. The setup leverages sustainable cloud infrastructure provided by Leafcloud.

## Repository Contents

- **helmfile.yaml**: Configuration file for managing Helm charts required for the LLM setup.
- **utils-chart/**: Custom helm chart for some infra need for this stack.


## Key Components

- **Managed Kubernetes Cluster with Gardener**: Platform for running the LLM model.
- **Ollama**: Tool for running large language models efficiently within Kubernetes.
- **AnythingLLM**: User interface for interacting with the LLM model.
- **Ingress NGINX**: Manages incoming traffic to the LLM setup.
- **Certbot**: Automates SSL certificate management.
- **chromadb**: Stores LLM embeddings for document-based model customization.

## Installation Steps

1. **Create Kubernetes Cluster**: Follow instructions in the `docs/` directory.
2. **Install Nvidia Drivers and CUDA Toolkit**: Use the Nvidia Kubernetes Operator.
3. **Assign Public Access**: Create subdomains for accessing the services.
4. **Streamlined Installation with Helmfile**: Use `helmfile.yaml` for installing necessary tools.
5. **Install Private LLM Environment**: Run `helmfile apply` to set up the environment.

For detailed instructions, refer to the `docs/` directory.
