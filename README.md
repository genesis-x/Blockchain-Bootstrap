# GENESISX BOOTSTRAP <img src="https://genesisx.network/img/logo-small.png" alt="GenesisX Logo" width="50" height="auto">

### 1. Stop/shutdown your wallet client if it is running.
<br/>

### 2. Navigate to your GenesisX data directory as shown below:

#### Your GenesisX data directory stores your blockchain, configuration, wallet, and masternode data.  By default, they are located in the following locations for each OS type:

## Windows
Go to Start > Run > %APPDATA%\GenesisX

(Hidden folder "AppData" - [How to view hidden folders on Windows](https://www.howtogeek.com/howto/windows-vista/show-hidden-files-and-folders-in-windows-vista/))


## OSX (MacOS)
Open a finder window, then select the "Go" dropdown menu. In this menu please press the "Go to Folder..." option. In the window that opens type: ~/Library/Application Support/GenesisX and press enter.

## MacOS High Sierra Only
/Users/YourUserName/.genesisx

<br/>

### 3. Delete ONLY the 4 folders and 1 file shown below:
### (blocks, chainstate, sporks, zerocoin, and peers.dat) folders from your data directory.
### (**Do NOT delete backups or wallet.dat**)

<img src="http://downloads.genesisx.network/folder.png" alt="GenesisX Folder" width="450" height="auto">

### 4. Download the latest bootstrap from [here](http://downloads.genesisx.network/bootstrap.zip)
### 5. Extract the bootstrap zip file you just downloaded to your desktop or elsewhere and you will see a file called "bootstrap"
### 6. Open the "bootstrap" file and drag all contents into your GenesisX data directory
### 7. Start your wallet client.
