# test-renovate

This repo aim to test the renovate configurations with monorepo, 
with the dependencies published from [test-renovate-packages](https://github.com/nandiheath/test-renovate-packages) 

## Running Renovate Locally

```bash
npm install
```

## Setup GH Personal Access Token

Generate Personal Access Token via the [portal](https://github.com/settings/tokens?type=beta). 
Make sure to grant the repo read permissions, and R/W for pull requests.

```shell
export GITHUB_TOKEN=<GH_PAT>

LOG_LEVEL=debug renovate --token=$GITHUB_TOKEN --labels=renovate,dependency --dry-run nandiheath/test-renovate  --dry-run 
```
