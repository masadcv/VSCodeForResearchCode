# VSCodeForResearchCode
A guide for setting up VSCode for research related coding tasks. This guide assumes you are using Ubuntu.

## Setting up python environment
- Install virtualenv package
```` bash
sudo apt install python3-virtualenv
````
- Create virtualenv in a known location
````bash
virtualenv /opt/virtualenvs/venv -p python3
````

## Install VSCODE and configure for python
- Download latest debian package from: https://code.visualstudio.com/
- Install using the dpkg as follows:
````bash
sudo dpkg -i code_*.deb
````
### Setting virutalenv folders for list of interpreters for VSCODE
Often on a prototyping workstation, it is helpful to use a single testing virtualenv as it speeds up setting up things.
To make a default virtualenv accessing in all new projects, update the following field in your user settings.json
- Go to settings **ctrl+,**
- Open **settings.json** from top right corner file icon
- Append json with entry
  ```` bash
  "python.pythonPath": "/opt/virtualenvs/venv/bin/python3"
  ````
- Save and reload

### Setting virutalenv folders for list of interpreters for VSCODE
- Go to settings **ctrl+,**
- Search **virtualenv**
- Write path **/opt/virtual_env**
- Save

### Useful VSCode extensions
- python extension: ms-python.python
- remote development: ms-vscode-remote.vscode-remote-extensionpack
- bracket pair coloriser: coenraads.bracket-pair-colorizer-2
- git lens: eamodio.gitlens

### Nice to have VSCode extensions
- material icons: pkief.material-icon-theme
- reload: natqe.reload
- resource monitor: mutantdino.resourcemonitor
- nvidia-smi: innerlee.nvidia-smi

### Copying keybindings for default VSCode shortcuts
- Use one of the default keybinding files saved within this folder
- Follow steps `Ctrl+K Ctrl+S` to access keybindings json [further help here](https://stackoverflow.com/a/60091222)
- Copy keybindings from provided json to the one on your VSCode system
