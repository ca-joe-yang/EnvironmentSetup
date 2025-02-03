# EnvironmentSetup

## Anaconda

### Installation
- Download Anaconda Installer
```shell
mv <ANACONDA_INSTALLER.sh> ~
cd ~
bash <ANACONDA_INSTALLER.sh>
```
- Add the following lines to `~/.bashrc`
```bash
PATH=$PATH:/home/<USER>/anaconda3/bin
```
- Source
```
source ~/.bashrc
```

### Create with basic packages
```
conda create -n <ENV_NAME> python=3.12 opencv pytorch torchvision torchaudio pytorch-cuda=12.1 yacs numba tqdm matplotlib seaborn scikit-image -c conda-forge -c pytorch -c nvidia -c
```

### Export
```
conda env export | grep -v "^prefix: " > environment.yml
```

## Visual Studio Code Extensions
- Remote-SSH

## Useful commands

### Deb installation
```shell
sudo dpkg -i <PACKAGE_NAME.deb>
```


### Github Enterprise
```bash
gh auth login -w
gh auth token
git clone https://${token}@github.com/${enterprise_name}/${repo_name}.git
```

### Mac
- install brew
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
- install `zsh`
```bash

```

