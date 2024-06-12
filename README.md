[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/sigscale-im)](https://artifacthub.io/packages/search?repo=sigscale-im)

# im-helm
Helm chart for deploying SigScale RIM on Kubernetes

## Deploy a SigScale RIM StatefulSet
	helm install im-1 sigscale-im

## List Helm releases
	helm list

## Remove a SigScale RIM StatefulSet
	helm uninstall im-1

## Deploy with localization overides in sys.config
	helm install \
			--set imConfig.create=true \
			--set-file imConfig.sysConfig=sys.config \
			im-1 sigscale-im

