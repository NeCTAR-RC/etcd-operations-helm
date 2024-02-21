# etcd-defrag

Sets up a cronjob to defrag etcd pods running in cluster. Optionally
backs up pre-defrag to an existing static or dynamically created pvc.

The job runs on a control plane node and ensures cluster health after
each node is defragmented and targets the leader last.

