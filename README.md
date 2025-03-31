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
  * At line 11, change the seven-digit number to your RIC/CAP-code
  * Also on line 11, ensure you have the correct location for the `rpitx pocsag` software
  * The `-f` flag on line 11 is the frequency to transmit on. It is set to 439.9875MHz (the defaut pager frequency for amateur radio in the UK) - but you can change this to any frequency. *Be sure to only transmit on frequencies you are either licensed for, or which are license-free!* It is your responsibility to stay within the law.
  * Line 13 is the confirmation message which you can change to your choosing.

## Usage
To run the script, simply type `pager` at the command line. Doing this will display the help information.

Ordinarily you would type `pager "{messageHere}"` and press return, and the message would send.

I hope you find this script helpful, and that it saves you time.

73 Michael GM5AUG
