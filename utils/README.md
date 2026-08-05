# Utility Scripts

Standalone helper scripts for building and provisioning outside of the `im-train-demo` workflow.

## build-and-push.sh

Builds all container images from their git tags and pushes them to a registry. Useful for CI or one-off builds without the interactive demo flow.

```bash
./utils/build-and-push.sh --help
```

## create-vm.sh

Creates a single libvirt VM from a qcow2 image with cloud-init hostname configuration. Hardcoded defaults — edit the variables at the top of the script to match your environment.

```bash
./utils/create-vm.sh
```

For the full interactive demo workflow (infrastructure setup, builds, deployments, and upgrades), use `im-train-demo` instead. See [INSTRUCTOR_GUIDE.md](../INSTRUCTOR_GUIDE.md) for the step-by-step walkthrough.
