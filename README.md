# Helm Charts Repository

Welcome to the `boveloco/charts` repository! This repository hosts all Helm charts maintained by **boveloco** for deploying various applications and services on Kubernetes.

## Table of Contents
- [Usage](#usage)
- [Charts](#charts)
- [Installation](#installation)
- [Contributing](#contributing)
- [License](#license)

## Usage

To use the Helm charts from this repository, add it as a Helm repository:

```sh
helm repo add boveloco https://boveloco.github.io/charts
helm repo update
```

## Charts

This repository contains the following Helm charts:

| Chart Name  | Description |
|-------------|------------|
| `common` | This chart is an interface for common simple deployments. |
| `ntp` | This chart deploys an NTP server. Forked from [GlennHD](https://github.com/GlennHD/kube-chrony)|

Check each chart’s documentation in its respective folder for installation instructions and configuration options.

## Installation

To install a chart, run:

```sh
helm install my-release boveloco/<chart-name>
```

To customize values, create a `values.yaml` file and install with:

```sh
helm install my-release boveloco/<chart-name> -f values.yaml
```

## Contributing

Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`feature/new-chart`).
3. Add/update Helm charts.
4. Submit a pull request.

## License

This repository is licensed under the [MIT License](LICENSE).