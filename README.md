# nutspawn

Better `spawn.nut`. Kinda messy atm, might make a clean PR to Northstar main later.

`original.nut` is there for comparison, eg. run:

    $ diff --color original.nut spawn.nut

for code changes.

# Installation

Copy `spawn.nut` to `R2Northstar/mods/Northstar.CustomServers/mod/scripts/vscripts/mp/spawn.nut` in your Northstar folder

# Changes

 * added 20 meter minimum enemy distance to spawnpoint validator (previously none)
 * spawnpoint is valid now after 5 second last use time (instead of 10 seconds)
 * valid spawn point sample size is 5 (previous was 3)
 * valid spawn point samples are sorted by distance to average team location, and the closest one is picked (instead of random), this should lead to slightly more teamplay
