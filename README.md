# kubezone

This repository is a centralized plugin index for kubectl plugins. Learn more about kubectl plugins here.

## Currently indexed plugins -
* backup-diff


## Usage

### Pre-requisistes -
* krew - check out this guide on how to install krew

Install via Krew

```shell

kubectl krew index add kubezone https://github.com/milapj/kubezone

kubectl krew index list

kubectl krew install kubezone/backup-diff
