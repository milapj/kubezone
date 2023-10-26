# kubezone

This repository is a centralized plugin index for kubectl plugins. Learn more about kubectl plugins [here](https://kubernetes.io/docs/tasks/extend-kubectl/kubectl-plugins/).

## Currently indexed plugins
* [backup-diff](https://github.com/milapj/kubectl-backup-diff)


## Usage

### Pre-requisistes
* [krew](https://krew.sigs.k8s.io/) - check out [this](https://krew.sigs.k8s.io/docs/user-guide/setup/install/) guide on how to install krew

## Install via Krew

1. Add kubezone index to krew
    ```console
    $ kubectl krew index add kubezone https://github.com/milapj/kubezone
    ```
1. Verify kubezone index is added
    ```console
    $ kubectl krew index list
    INDEX    URL
    default  https://github.com/kubernetes-sigs/krew-index.git
    foo      https://github.com/foo/custom-index.git
    ```
1. Install plugin indexed in kubezone
    ```console
    $ kubectl krew install kubezone/backup-diff
    Updated the local copy of plugin index.
    Updated the local copy of plugin index "kubezone".
    Installing plugin: backup-diff
    Installed plugin: backup-diff
    \
    | Use this plugin:
    |      kubectl backup-diff
    | Documentation:
    |      https://github.com/milapj/kubectl-backup-diff
    /
    ```

## Bug Reports

If you're having an issue with an installed plugin itself, file an issue for the repository the plugin's source code is hosted at.
