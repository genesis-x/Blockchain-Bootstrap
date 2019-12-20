<img src="downloads.genesisx.network/bootstrapHeaderImage.png" min-width="250" height="auto">

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

<br/>

## FAQ

### Q:
My wallet seems to have become stuck syncing and says remains at X hours left. It’s been many hours and status hasn't changed. What do I do?

### A:
This may happen due to connecting to some bad peers or your chain has been corrupted somehow.
First, try simply restarting the wallet then after it's synced up, check if you are on the right chain via a block explorer: <br/>
[Explorer 1](http://xgs.ccore.online/) <br/>
[Explorer 2](http://45.77.214.49/) <br/>
If you are on the right chain but isn't syncing the newer blocks, please follow solution steps outlined
below to resync cleanly off the network with a new peers.dat: <br/>

Inside GUI Wallet: <br/>
"Tools > Wallet Repair > Delete Local Blockchain Folders (-resync)" to initiate the full re-sync. <br/>
(unless you have a known good backup of the blockchain that you know how to restore)

Also, ensure that your genesisx.conf doesn't have any connect= or addnodes= lines unless you know why they are there. 
