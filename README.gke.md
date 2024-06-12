# Manage Google Kubernetes Engine (GKE)

## Create a GKE Autopilot Cluster
	gcloud container clusters create-auto im-cluster

## Configure `kubectl` to use the GKE Cluster
	gcloud container clusters get-credentials im-cluster

$# Get the Pods (after `helm install`)
	kubectl get pods

## Get the log of init container
	kubectl logs im-1-sigscale-im-0 -c im-init

## Get the log of container
	kubectl logs im-1-sigscale-im-0

## Describe the pod
	kubectl describe pod im-1-sigscale-im-0

## Attach to a GKE pod deployment which runs im container
	$ kubectl attach -ti im-1-sigscale-im-0 -c im -i -t
	(im@im-1-sigscale-im-0.otp-im.default.svc.cluster.local)5>
### There is no `detach` so you'll need to kill the `kubectl attach` process

