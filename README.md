# Poollogs-cleanup
Cleanup script for Dpos poollog.json (by Dakk) used for delegate pay-out in lisk/shift/ARK/rise/oxy/lwf/kapu/onz etc 

This script

## Configuration / prerequisists
This script asumes that you have installed the "Lisk pool distribution software" by Dakk.
It uses the information from the config.json which was created during the Lisk pool setup and reads, cleans and rewrites the poollogs.json.

## Running it
First clone the Poollogs-cleanup repository (I asume you already have installed the Lisk pool and requests):

`git clone https://github.com/dwarf-forging/poollogs-cleanup`

`cd poollogs-cleanup`


Then start it:

`python3 poollogs-cleanup.py`

or if you are using another config file:

`python3 poollogs-cleanup.py -c config2.json`

It produces 2 files 
`First file is called "removed-voters.json" with all the removed voters with their payout and pending payout (it is in the same format as the poollogs.json
`Second file is the cleaned poollogs.json

You can move (or copy) this generated removed-voters.json to the directory docs.
