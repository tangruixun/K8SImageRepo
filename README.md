# K8SImageRepo

Get K8S Images from GHCR (GitHub Container Registry)

The general command syntax is:

    <Command> pull ghcr.io/tangruixun/<PackageName>-<Tag>:<Tag>
    <Command> [-n k8s.io image] tag ghcr.io/tangruixun/<PackageName>-<Tag>:<Tag> registry.k8s.io/<PackageName>:<Tag>

e.g. If you need `registry.k8s.io/pause:3.6`:

- Docker:

      docker pull ghcr.io/tangruixun/pause-3.6:3.6
      docker tag ghcr.io/tangruixun/pause-3.6:3.6 registry.k8s.io/pause:3.6

- cricrl/ctr:

      crictl pull ghcr.io/tangruixun/pause-3.6:3.6
      ctr -n k8s.io image tag ghcr.io/tangruixun/pause-3.6:3.6 registry.k8s.io/pause:3.6

All current packages list can be found [here](https://github.com/users/tangruixun/packages?repo_name=K8SImageRepo).

Please replace `registry.k8s.io` with `k8s.gcr.io` for very old k8s installation.

Support me on Paypal: [![Support me on Paypal](hhttps://www.paypalobjects.com/paypal-ui/logos/svg/paypal-color.svg)](https://paypal.me/tangruixun?country.x=C2&locale.x=en_US)
 <>
