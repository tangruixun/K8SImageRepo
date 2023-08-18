# K8SImageRepo

Get K8S Images from GHCR (GitHub Container Registry)
	
The general command syntax is:

    <Command> pull ghcr.io/tangruixun/<PackageName>-<Tag>:<Tag>
    <Command> [-n k8s.io image] tag ghcr.io/tangruixun/<PackageName>-<Tag>:<Tag> registry.k8s.io/<PackageName>:<Tag>
	
e.g. If you need `registry.k8s.io/pause:latest`:

- Docker:

      docker pull ghcr.io/tangruixun/pause-latest:latest
      docker tag ghcr.io/tangruixun/pause-latest:latest registry.k8s.io/pause:latest

- cricrl/ctr:

      crictl pull ghcr.io/tangruixun/pause-latest:latest
      ctr -n k8s.io image tag ghcr.io/tangruixun/pause-latest:latest registry.k8s.io/pause:latest
	
All current packages list can be found [here](https://github.com/users/tangruixun/packages?repo_name=K8SImageRepo).

Please replace `registry.k8s.io` with `k8s.gcr.io` for very old k8s installation.
