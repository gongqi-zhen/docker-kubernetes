
# create GKE cluster
# 20210528


```
% gcloud container clusters create demo-cluster --cluster-version=1.19.9-gke.1400 \
> --machine-type=n1-standard-1 \
> --num-nodes=3
WARNING: Currently VPC-native is not the default mode during cluster creation. In the future, this will become the default mode and can be disabled using `--no-enable-ip-alias` flag. Use `--[no-]enable-ip-alias` flag to suppress this warning.
WARNING: Starting with version 1.18, clusters will have shielded GKE nodes by default.
WARNING: Your Pod address range (`--cluster-ipv4-cidr`) can accommodate at most 1008 node(s).
WARNING: Starting with version 1.19, newly created clusters and node-pools will have COS_CONTAINERD as the default node image when no image type is specified.
Creating cluster demo-cluster in asia-northeast1-a... Cluster is being health-checked (master is healthy)...done.
Created [https://container.googleapis.com/v1/projects/xxxxx/zones/asia-northeast1-a/clusters/demo-cluster].
To inspect the contents of your cluster, go to: https://console.cloud.google.com/kubernetes/workload_/gcloud/asia-northeast1-a/demo-cluster?project=gke-test-314015
kubeconfig entry generated for demo-cluster.
NAME          LOCATION           MASTER_VERSION   MASTER_IP      MACHINE_TYPE   NODE_VERSION     NUM_NODES  STATUS
demo-cluster  asia-northeast1-a  1.19.9-gke.1400  xxx.xxx.xxx.xxx  n1-standard-1  1.19.9-gke.1400  3          RUNNING
makoto@miyazakimakotonoMacBook-Pro ~ %
```
