# discoaccountswitcher
A small utility to switch your Discovery Freelancer accounts on Linux


## Requirements

- Bash
- xmlstarlet
- Wine
- A working wine prefix for your discovery install
- A working discovery install (duh)

## Setup

You need to edit the script so that it points to both your discovery wine prefix (the one with dotnet40 installed) and your path to the wine version you use to run the game (staging 2.21 if you followed my guide)

It is important that you modify the script in the following manner:

- The `prefix` line should point to the wine prefix you use to run the game, otherwise you're modifying the wrong files with this account switcher. It should look like the following:
`prefix=/home/user/.winedisco`
- The `wine` line should be the wine executable for wine-staging 2.21, wherever you decided to install that to. It should look like the following:
`wine=/path/to/staging-2.21-x86_64/bin/wine`

## Usage

`./launcher <your launcheraccts.xml> <option> <selection>`

- Your options are list and select
- Selection is the account number, you can find out which account number you need from the list
