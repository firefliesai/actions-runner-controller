# Build Runner Image

To build Runner Image for fireflies-ai usages, simply execute the following commands

```bash
DOCKER_USER=ghcr.io/firefliesai/infra-toolbox TARGETPLATFORM=amd64 make docker-build-default docker-push-default
```

Make sure you have Docker installed, and you're using x86 machine.

# Update Runner Image version

To reflect the changes to our CI flow, updates the Runner instance like [this one](https://github.com/firefliesai/k8s-staging/blob/main/action-runner-system/runners/dashboard-ff.runner.yaml#L8) to the desired image version.