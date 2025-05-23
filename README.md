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
**Step 3:** Run the Install script. To run the script, run:
  ```
  python3 txsearch-inst.py
  ```
  # Usage
  After you have installed TxSearch with the Install Script, you will need to know how to use it. To open TxSearch, run:
  ```
  python3 txsearch.py
  ```
  You will be granted with this prompt:
  ```
  1: lo: <LOOPBACK,UP,LOWER_UP> mtu xxxxxx qdisc noqueue state UNKNOWN group default qlen xxxx
    link/loopback xx:xx:xx:xx:xx:xx brd xx.xx:xx:xx:xx:xx
    inet xxx.x.x.x/x scope host lo
       valid_lft forever preferred_lft forever
    inetx ::x/xxx scope host noprefixroute 
       valid_lft forever preferred_lft forever
  4: wlp3sx: <BROADCAST,MULTICAST> mtu xxxx qdisc noop state DOWN group default qlen xxxx
    link/ether xx:xx:xx:xx:xx:xx brd xx:xx:xx:xx:xx:xx permaddr xx:xx:xx:xx:xx:xx
  5: xxxxxxxxxxxxxxx: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu xxxx qdisc fq_codel state UP group default qlen xxxx
    link/ether xx:xx:xx:xx:xx:xx brd xx:xx:xx:xx:xx:xx
    inet xxx.xx.xx.x/xx brd xxx.xx.xx.xx scope global dynamic noprefixroute xxxxxxxxxxxxxxx
       valid_lft xxxxsec preferred_lft xxxxsec
    inetx xxxx:xxx:xxxx:xxxx:xxxx:xxxx:xxx:xxxx/xx scope global noprefixroute 
       valid_lft forever preferred_lft forever
    inetx xxxx::xxxx:xxxx:xxxxxxxxx/xx scope link noprefixroute 
       valid_lft forever preferred_lft forever
  ```
  These characters are info about your network
  "Are these details correct?(y/n)" Enter "n" if not. Enter "y" if you do not know or you are sure.
  You will next be granted with this:
  ```
  Select a search engine:
  Google(firefox)
  Google(firefox--privite-window)
  Brave(brave-browser)
  Brave(brave-browser --incognito)
  Tor(brave-browser --tor)

  NOTE: Must have installed selected browser!

  NUMBER:
  ```
  Enter the number (line) of the search engine you want.
  Next enter your URL from the next input. And you are done.
  # Uninstallation
  Run the following command:
  ```
  sudo rm -rf /home/user/txsearch.py && sudo rm -rf /home/user/txsearch-inst.py
  ```
  Of course, replace the directories with YOUR path.
