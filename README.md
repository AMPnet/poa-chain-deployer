# poa-chain-deployer
AMPnet PoA Besu deployer script.

## Requirements

Make sure you have following installed on your local environment:
* [Helm](https://helm.sh/docs/)
* [Helmfile](https://github.com/roboll/helmfile)
* [Helm Diff plugin](https://github.com/databus23/helm-diff)

Helm Charts are used to deploy all of the necessary components of the system.
It is also assumed there's a working [kubectl tool](https://kubernetes.io/docs/reference/kubectl/) installed and properly configured to be connected to your local or remote kubernetes cluster.

Helm version tested an working with this script is v3.4.2. Check the helm version by running

```
# outputs helm version info
helm version
```

Kubectl version tested and working with this script is client-version@1.23.3 and server-version@1.22.7. Check the kubectl version by running 

```
# outputs kubectl client and host version
kubectl version
```

Check if the kubernetes cluster is reachable and healthy (If you see a URL response, kubectl is correctly configured to access your cluster):
```
kubectl cluster-info
```

## Steps to deploy PoA network

The following defines the steps required to deploy your own PoA network.

### Step 1: Deploy genesis config

// TODO

### Step 2: Deploy validators

// TODO

### Step 3: Deploy block explorer

// TODO

### Step 4: Deploy ingress and expose ports

// TODO

## Automated deployment

PoA network can be deployed automatically by configuring the values in the `deployment.yaml` and then calling the script
```
./deploy.sh
```
// TODO: rewrite this section once the deployment script and the config file have been fully defined
