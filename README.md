# TxSearch
Free, text based browser launcher. Made for Debian versions supporting Python3 and Brave-Browser. Made on Debian 12.11 Bookworm. Read install page for more info!
# Installation
Install page for TxSearch on Debian. Must have:
- Debian Advanced Package Tool (apt)
- Python 3 (python3)
- GitHub Cloning (git)
- Modzilla Firefox (firefox)
Additionally, but recomended:
- Brave Browser (brave-browser)
**Install Python**
  In order to run the Python script to download Firefox or Brave, we need to download Python itself. First you need to update your avalible packages and update your packages.
**Update avalible packages (to get newest python version)**
```
sudo apt-get update && sudo apt-get upgrade
```
Next is the command to install python.
**Install Python 3**
```
sudo apt-get install python3
```
**TxSearch Installation Script**
Step 1: Make sure you have Python installed. Run:
```
python3 --version
```
Once entered, output should look simular too:
```
Python 3.x.x
```
Step 2: Install TxSearch Install Script. This is the easiest way of installing FireFox and Brave. You will need GitHub Cloning.
First, **Install git.** Run:
```
sudo apt-get install git
```
The "git" command will allow you to clone repositories from GitHub. Next install "wget", which will allow you to install single scripts from GitHub. Since "git clone" can only clone repositories, we need to get raw files with "wget". Run:
```
sudo apt-get install wget
```
Finally, to **get the install script,** run:
```
wget https://raw.githubusercontent.com/roccohimel/txsearch/refs/heads/main/txsearch-inst.py
```
**This will:**
- Install FireFox ESR
- Install Brave
- Install the TxSearch script
