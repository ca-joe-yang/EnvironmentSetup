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

### Create
```
conda create -n <ENV_NAME> python=<VERSION>
conda activate <ENV_NAME>
conda install pytorch torchvision -c pytorch
```

### Basic Packages
```
conda install -c conda-forge opencv ipython tqdm yacs matplotlib
conda install -c anaconda scikit-image
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
