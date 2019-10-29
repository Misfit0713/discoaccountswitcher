# discoaccountswitcher
A small utility to switch your Discovery Freelancer accounts on Linux


## Requirements

- xmlstarlet
- Wine
- A working wine prefix for your discovery install
- A working discovery install (duh)

## Setup

You need to edit the script so that it points to both your discovery wine prefix (the one with dotnet40 installed) and your path to the wine version you use to run the game (staging 2.21 if you followed my guide)

It is important that you modify the script in the following manner:

- The `prefix` line should point to the wine prefix you use to run the game, otherwise you're modifying the wrong files with this account switcher. It should look like the following:
`prefix="/home/user/.winedisco"`
- The `wine` line should be the path to the bin directory for wine-staging 2.21, wherever you decided to install that to. It should look like the following:
`wine="/path/to/staging-2.21-x86_64/bin/"`
- The `acct` line should point to your launcheraccounts.xml file. It should look like the following:
`acct="/path/to/launcheraccounts.xml"`

## Usage

`./launcher <option> <selection>`

- Your options are list and select (and launch if you've set it up)
- Selection is the account number, you can find out which account number you need from the list

## Additional functionality

If you have a script to launch the game with, you can also use the launch option to call that script. It's the last if statement if you'd like to put your preferred method for launching the game there.
