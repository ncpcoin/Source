## NCPCoin Wallet 

### Overview 

If you are a newcomer, check out the [NCPCoin website](https://ncpcoin.org/) which explains NCPCoin in simple and everyday terms. You can find statistics on the current state of the NCPCoin research rates on the [Team Stats Page](https://folding.extremeoverclocking.com/team_summary.php?s=&t=224497) and blockchain status and info on the [NCPCoin Block Explorer](https://chainz.cryptoid.info/ncpcoin/)

### Joining the NCPCoin network is easy:
On Windows, the [All-In-One FoldingBrowser Installer](https://github.com/Hou5e/FoldingBrowser/releases) provides a quick setup for running Folding@home to earn both NcpCoin and FoldingCoin.

### Or, setup for getting NCPCoin only for running Folding@home with any username:
1. Install the [Folding@home software](https://foldingathome.org/start-folding/), or the [F@H Chrome Browser plugin](https://chrome.google.com/webstore/detail/foldinghome/hmnbjdgjgikbkapaolimfoidihobnofo) (CPU only, better for lower power laptops)
2. Pick a Folding@home Username & get a [Passkey](https://apps.foldingathome.org/getpasskey)
3. Enter "224497" as the Team number to fold under
4. Register on [cryptobullionpools.com](https://www.cryptobullionpools.com/) with the **exact** same username (50 characters or less) used in Folding@home
5. Expect your CureCoins within 24-32 hours!

## Standard Wallet Installation

[CureCoin GitHub Releases](https://github.com/ncpcoin/releases) has the Windows, Mac, Linux wallet downloads.  
**CureCoin v2.0 is a mandatory update.** Older wallets need to be updated to this version (or newer) to work correctly.

## Linux Installation From Source

If you do not use Linux, see previous section for a prebuilt wallet. There are two CureCoin Linux based clients that you can compile for yourself: one with a nice graphical interface, and one that operates entirely in the command-line. The first is highly recommended and is a good choice for most users, but expert users may prefer the command-line (headless) client instead. The GUI client is known as "curecoin-qt" and the headless client is called "curecoind". Installing either one or both is extremely simple. Just follow these directions:

- **Install Steps For Linux**

    This involves downloading the source, meeting the dependencies, compiling the code, and then installing the resulting software.

    git clone https://github.com/ncpcoin/Source.git

    ### FOR THE GUI CLIENT:
    > 1. **sudo apt-get install qt5-default qt5-qmake qtbase5-dev-tools qttools5-dev-tools libboost-dev libboost-system-dev libboost-filesystem-dev libboost-program-options-dev libboost-thread-dev libssl-dev libminiupnpc-dev libdb5.3++-dev dh-make build-essential** &nbsp; &nbsp; &nbsp; &nbsp; {See: **NOTES** below}
    > 2. From the main directory, run the following:
    > 3. **qmake && make**

    ### FOR THE HEADLESS CURECOIND:
    > 1. **sudo apt-get install libboost-all-dev libqrencode-dev libssl-dev libdb5.3-dev libdb5.3++-dev libminiupnpc-dev dh-make build-essential** &nbsp; &nbsp; &nbsp; &nbsp; {See: **NOTES** below}
    > 2. **cd src**
    > 3. **make -f makefile.unix**
    > 4. **sudo make install** &nbsp; &nbsp; {Alternatively, don't run that command, and just place the binary wherever you want}

    ### NOTES:
    - On new versions of Linux such as Ubuntu 18.04 or Debain 9, additionally install: "sudo apt-get install libssl1.0-dev"
    - On older Linux versions, like Ubuntu 14.04, use: libdb4.8 or libdb5.1. Newer Ubuntu 16.04, use: libdb5.3++-dev.

### Linux Example: Typical CureCoin GUI Wallet Install Steps on Mint 19:
```
sudo apt install git
sudo apt-get install qt5-default qt5-qmake qtbase5-dev-tools qttools5-dev-tools libboost-dev libboost-system-dev libboost-filesystem-dev libboost-program-options-dev libboost-thread-dev libssl-dev libminiupnpc-dev libdb5.3++-dev dh-make build-essential

sudo apt-get update
sudo apt-get upgrade
sudo apt-get install libssl1.0-dev
[Reboot]  -NOTE: 'libssl1.0-dev' needs to be installed *after* installing the other dependencies at the beginning. If the dependencies at the beginning fail, then make sure you have updates enabled and the PC is fully updated.

mkdir curecoin
cd curecoin

git clone https://github.com/ncpcoin/Source.git
cd CurecoinSource
qmake
make
./curecoin-qt
```

### Reporting Bugs or Getting Assistance

Ask questions on the [NCPCoin Discord](https://discord.gg/mtztkFZ). Other general help can be searched for on the [NCPCoin forums](https://ncpcoin.org/forum/).

### Donations

Stars on this repo are appreciated as it helps improve the visibility of this repository. If you'd like to do more than that, you can tip CureCoins on the [NCPCoin website](https://ncpcoin.org/).
