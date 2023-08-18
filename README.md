# K8SImageRepo

Get K8S Images from GHCR (GitHub Container Registry)

e.g. If you need `k8s.gcr.io/pause:latest`:

Docker:

    docker pull ghcr.io/tangruixun/pause-latest:latest
    docker tag ghcr.io/tangruixun/pause-latest:latest registry.k8s.io/pause:latest

cricrl/ctr:

    crictl pull ghcr.io/tangruixun/pause-latest:latest
    ctr -n k8s.io image tag ghcr.io/tangruixun/pause-latest:latest registry.k8s.io/pause:latest
	
The general command synax is:

    <Command> pull ghcr.io/tangruixun/<PackageName>-<Tag>:<Tag>
	<Command> [-n k8s.io image] tag ghcr.io/tangruixun/<PackageName>-<Tag>:<Tag> registry.k8s.io/<PackageName>:<Tag>

All current packages can be found at [here](https://github.com/users/tangruixun/packages?repo_name=K8SImageRepo).
