---
title: "Installation"
description: "OCM Controller Installation"
draft: false
images: []
weight: 42
toc: true
---

## ocm-controller

The `ocm-controller` can be installed using the [OCM CLI](/docs/getting-started/installing-the-ocm-cli):

```bash
ocm controller install
```

This command will install the `ocm-controller` in the kubernetes cluster specified by the current `KUBECONFIG` context.

The following flags are available:

```bash
Flags:
  -u, --base-url string          the base url to the ocm-controller's release page (default "https://github.com/open-component-model/ocm-controller/releases")
  -c, --controller-name string   name of the controller that's used for status check (default "ocm-controller")
  -d, --dry-run                  if enabled, prints the downloaded manifest file
  -h, --help                     help for install
  -n, --namespace string         the namespace into which the controller is installed (default "ocm-system")
  -a, --release-api-url string   the base url to the ocm-controller's API release page (default "https://api.github.com/repos/open-component-model/ocm-controller/releases")
  -t, --timeout duration         maximum time to wait for deployment to be ready (default 1m0s)
  -v, --version string           the version of the controller to install (default "latest")

Description:
  Install either a specific or latest version of the ocm-controller.
```
