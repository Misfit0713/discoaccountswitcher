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

## Usage

`./launcher <your launcheraccts.xml> <option> <selection>`

- Your options are list and select
- Selection is the account number, you can find out which account number you need from the list
