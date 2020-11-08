<img src="http://downloads.genesisx.network/bootstrapHeaderImage.png" min-width="750" height="auto">

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

### 4. Download the latest bootstrap from [here](https://ln2.sync.com/dl/2af65f300/4tyidsbi-hyj7dsg3-f3i8f8n8-9ff4en4a)
### 5. Extract the bootstrap rar file you just downloaded to your desktop or elsewhere and you will see a file containing the word "bootstrap".
### 6. Open the "bootstrap" file and drag all contents into your GenesisX data directory.
### 7. Start your wallet client.

<br/>

## FAQ

### Q:
Is this safe?

### A:
Yes, the above method is safe. The download contains only raw blockchain data and the client verifies this on import. Do not download the blockchain from unofficial sources, especially if they provide *.rev and *.sst files. These files are not verified and can contain malicious edits.


### Q:
My wallet seems to have become stuck syncing and says remains at X hours left. It’s been many hours and status hasn't changed. What do I do?

### A:
This may happen due to connecting to some bad peers or your chain has been corrupted somehow.
First, try simply restarting the wallet then after it's synced up, check if you are on the right chain via a block explorer: <br/>
[Explorer 1](http://xgs.ccore.online/) <br/>
[Explorer 2](https://chains.trittium.cc/XGS/blocks) <br/>
If you are on the right chain but isn't syncing the newer blocks, please follow solution steps outlined
below to resync cleanly off the network with a new peers.dat: <br/>

Inside GUI Wallet: <br/>
"Tools > Wallet Repair > Delete Local Blockchain Folders (-resync)" to initiate the full re-sync. <br/>
(unless you have a known good backup of the blockchain that you know how to restore)

Also, ensure that your genesisx.conf has valid connect= or addnodes=. We have added ones that we are running off. Remove if they no longer serve as accurate.

### Q:
How do i know i am on the right chain?

### A:
In wallet debug panel enter "getblockhash 1272456".
You should get the block hash of "4b797989abfe884b6df1e511279a9ce03c4749b6e2876328c1df175aa341058c"
If not you will need to resync the wallet with a new peers.dat file.


### Q:
Do I really need a bootstrap?

### A:
In short, no. The purpose of bootstrap is to provide an up-to-date blockchain without the time and resource intensive tasks of verifying each block and/or reindexing the blockchain.
