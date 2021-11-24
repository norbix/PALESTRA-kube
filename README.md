# NORBIX-KUBE

Portable workloads orchestrator within docker engine on-demand.

## General info

### Structure

- **kubeconfig** contains static hosting assets 2 render docs.

## TODO

- REPLACE

## Tools

### Taskfile 

Download Taskfile from <https://taskfile.dev> 4 your OS and add binary to your PATH.

List of configured tasks:

```shell
.\bin\task.exe -t ./Taskfile.yml -l   - Wintel
./bin/task -t ./Taskfile.yml -l       - Linux
```

### kubectl

**Wintel users must define variable in .env file.**


#### Kubectl Shell

If u have access 2 k8s cluster add config as a file '''kubeconfig''' (excluded within .gitignore)

```shell
.\bin\task.exe -t ./Taskfile.yml 0001-k8s:kubectl-shell   - Wintel
./bin/task -t ./Taskfile.yml 0001-k8s:kubectl-shell       - Linux
```

### helm/helmfile

#### Helm Shell

If u have access 2 k8s cluster add config as a file '''kubeconfig''' (excluded within .gitignore)

```shell
.\bin\task.exe -t ./Taskfile.yml 0001-k8s:helm-shell   - Wintel
./bin/task -t ./Taskfile.yml 0001-k8s:helm-shell       - Linux
```
