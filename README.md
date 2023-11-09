
# Gangway Helm Chart

## Overview

This Helm chart deploys Gangway, an application designed to facilitate authentication flows via OIDC for a Kubernetes cluster. 

- **apiVersion:** v2
- **name:** gangway
- **description:**
- **version:** 0.4.5
- **appVersion:** 3.3.0

## Dependencies

This chart has the following dependencies:

- **Name:** gangway
- **Version:** 0.4.5
- **Repository:** [https://charts.helm.sh/stable/](https://charts.helm.sh/stable/)

## Usage

To deploy Gangway, use the following Helm command:

```
helm install my-gangway-release stable/gangway
```

### Configuration

#### Namespace

Ensure that you have the `tools` namespace created before deploying Gangway. If not, create it using the following command:

```
kubectl create namespace tools
```

#### Gangway Configuration

Modify the `values.yaml` file or use Helm command-line options to customize the Gangway deployment. 

### Deploy Gangway

To deploy Gangway with the specified configuration, use the following Helm command:

```
helm install my-gangway-release -n tools stable/gangway -f values.yaml
```

For more configuration options and details, refer to the official Gangway documentation. (https://github.com/helm/charts/tree/master/stable/gangway)

### Notes

- Ensure that the necessary Kubernetes namespace (`tools`) is created before deploying Gangway.
- Customize the Gangway configuration based on your specific requirements.
- For detailed information about Gangway and its configurations, visit the official documentation: [Gangway Documentation](https://github.com/helm/charts/tree/master/stable/gangway)

