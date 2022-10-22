# experiment-install-sealos-in-actions

## Installers

- sealos: 
  - 未内置 helm 
  - 支持集群镜像
  - 需要使用专用版镜像支持 docker，不会自动安装 docker
  - 内存占用较大：1750M - 500M = 1250M
  - 速度较慢: 2m40s
- kubekey
  - 需要手动安装 socat, conntrack, ebtables, ipset 等依赖
  - 内置 helm 等
  - 支持 docker，可自动安装 docker
  - 速度较慢: 2m20s
  - 内存占用较小： 1350M - 500M = 850M
- k3s
  - 内置 helm 等
  - 速度快：<1m
  - 内存占用小： 1200M - 500M = 700M 
