# k8s-lab
This repo is to document my k8s lab in cloud

# Oracle Cloud Infrastructure - OCI

Oracle Cloud Infrastructure's Free Tier includes a free time-limited promotional trial that allows you to explore a wide range of Oracle Cloud Infrastructure products, and a set of Always Free offers that never expire. 

## How to setup k8s cluster into OCI

The bellow commands login to OCI from command lines (PowerShell) and downloads kube config locally. 

````
 oci ce cluster create-kubeconfig --cluster-id ocid1.cluster.oc1.uk-london-1.aaaaaaaa47sjh65hu3l5qx3jjom6fyhsjyijxya4qkz3wjqwqceoptoofh7q --file $HOME/.kube/config --region uk-london-1 --token-version 2.0.0  --kube-endpoint PUBLIC_ENDPOINT
````

## Cluster Varification:

Make sure you see the nodes as expected.

````
kubectl.exe get nodes

````