# K8SImageRepo

e.g. If you need `k8s.gcr.io/pause:latest`:

Docker:

    docker pull ghcr.io/tangruixun/pause-latest:latest
    docker tag ghcr.io/tangruixun/pause-latest:latest k8s.gcr.io/pause:latest

cricrl/ctr:

    crictl pull ghcr.io/tangruixun/pause-latest:latest
    ctr -n k8s.io image tag ghcr.io/tangruixun/pause-latest:latest k8s.gcr.io/pause:latest

All current packages can be found at [here](https://github.com/users/tangruixun/packages?repo_name=K8SImageRepo).
