# Kubernetes-notes

## Pods CPU and Memory Usage


If you want to check pods cpu/memory usage without installing any third party tool then you can get memory and cpu usage of pod from cgroup.

###Go to pod's exec mode kubectl exec -it pod_name -n namespace -- /bin/bash###
```Run cat /sys/fs/cgroup/cpu/cpuacct.usage for cpu usage
Run cat /sys/fs/cgroup/memory/memory.usage_in_bytes for memory usage```
