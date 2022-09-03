# TermuxPackageBuilder
A docker image for termux-builder, it is so easy to build package.

## What is TermuxPackageBuilder?
It provides a quick way to build multi-platform package.
If your device cannot download termux-builder image, please use this.

>How to use?
>First, install git.
```bash
# If your device is Linux, use "apt" package manager to install it.
apt install git

# If your device is Windows, please download the Git.
# The Git link: https://git-scm.com/
```

>Second, clone this depository.
```bash
git clone https://github.com/CaiMuCheng/TermuxPackageBuilder
```

>Third, install docker
```bash
# If your device is Linux, use "apt" package manager to install it.
apt install docker.io

# If your device is Windows, please download the "Docker Desktop".
# The Docker Desktop link: https://docs.docker.com/desktop/install/windows-install
```

>Fourth, install curl
```bash
# If your device is Linux, use "apt" package manager to install it.
apt install curl

# If your device is Windows, need not do it.
```

>Last, use "docker" command to start this image!
```bash
# This operation may take some time, please wait for it!
cd TermuxPackageBuilder && chmod 777 fetchFile.sh && ./fetchFile.sh && docker import package-builder.tar termuxPackageBuilder && docker run -t -i termuxPackageBuilder
```