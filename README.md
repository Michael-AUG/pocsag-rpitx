# pocsag-rpitx
Script to automate sending POCSAG messages using rpitx

## Introduction
This script builds on the excellent [rpitx](https://github.com/F5OEO/rpitx) software created by F5OEO, and offers a simple way to automate sending POCSAG (PAGER) messages using his software.

## Installation
* `git clone https://github.com/Michael-AUG/pocsag-rpitx`
* `cd pocsag-rpitx`
* `sudo mv ./pager /usr/local/bin`

## Configuration
In order to run the script, you will need to make a couple of changes.
* Edit the script (`sudo nano /usr/local/bin/pager`)
  * Edit `RIC` (line 5) to your RIC code (obtained from DAPNET)
  * Edit `FREQ` (line 6) to the chosen frequency (Make sure you abide by local laws/licence conditions)
  * Edit `pocsagLocation` (line 7) to wherever rpitx is installed
  * Edit `CALLSIGN` (line 8) to your callsign for confirmation

## Usage
To run the script, simply type `pager` at the command line. Doing this will display the help information.

Ordinarily you would type `pager "{messageHere}"` and press return, and the message would send.

I hope you find this script helpful, and that it saves you time.

73 Michael GM5AUG
