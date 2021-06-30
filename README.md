# Note

This repo is archived in favour of the bitcoin helm chart in lsdcapital/helm-charts/bitcoind

# Bitcoin Helm Chart

By default it has 500gi persistant storage mounted to /data (tested on GKE. Please help test on others)
There is no ingress route created, but internal ClusterIP for interprocess communications

## Configuration
The bitcoin.conf file is stored in config/bitcoin.core.sample. Rename this to bitcoin.core and adjust. You probably want to set the rpcuser and pass.

## Deploy
helm upgrade -i bitcoind .
