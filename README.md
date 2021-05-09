# No Loot Drops for Torchlight II

This Torchlight 2 mod makes enemies drop only gold, allowing you to focus solely on clearing while adventuring - leaving the item management and theorycrafting for when you're safely back in town. Why would a dog ever drop a sword or ring, anyways...?

This does not affect **anything** other than drops from normal monsters - so chests (and all other item containers), mimics, golden crabs, etc. are not affected. This initial release also does not change, in any way, drops from champion or boss monsters either.

With random loot still being generated by chests and other sources, this approach allows for the usual excitement of coming across epic gear (and the challenge of making the most out of that), while also promoting more intentional agency and strategy in your theorycrafting during minute-to-minute gameplay because you have to deliberately choose when and how to spend your gold rather than just picking incremental upgrades off of the ground.

## How to install

Download the latest version of the mod file from [the GitHub release page](https://github.com/tukkek/torchlight2-NoLootDrops/releases) and place it on your Torchlight 2 mod folder. If you're unsure the exact folder location, use the "Open mods folder" button on the official Mod Launcher tool. Check [this video](https://www.youtube.com/watch?v=e5KeocjLUiA) for step-by-step instructions.

Steam Workshop version pending.

## On balance

Balance has been tested this way, on Normal difficulty:

1. Run the first area of the game multiple times
2. Don't use consumables and ignore containers
3. Pick all monster drops
4. Make a straighforward bee-line to the end of the area
5. Sell all loot and gear once you reach the first town
6. Make note of the final amount of gold owned, deducing the value of the given starting items (~400 gold)
7. Take a median from all runs

The results:
* Vanilla: ~300 gold
* No Loot Drops: ~300 gold

For a number of reasons this isn't as "perfect" as the numbers initially suggest but further playtesting hasn't shown any major issues.

## What is changed?

1. The Spawn Class `TREASURE_MONSTERLOOT_NORMAL` now rolls on the `GOLD_PIECE` table instead of the `TREASURE` table. This is a very simple approach that does not take a couple technicalities under consideration but it seems to be balanced enough while also being maximally compatible with other mods.

## Possible future changes

1. Make champions and bosses also only drop gold (as long as balance and the chance for coming across cool gear from other sources is maintained).
2. ~~Consider boosting the amount of gold dropped, using the minimum- and maximum-rolls fields, to make up for having to depend more on expensive vendor purchases~~ (further testing shows this probably isn't necessary).
3. Steam Workshop page for more convenient installation.
