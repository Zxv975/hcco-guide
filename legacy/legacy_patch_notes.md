---
title: Legacy Patch Notes
layout: page
parent: Home
--- 

This is a historical page

 V0.0
"Official" HCCO release!

Adds an entirely new mode which is effectively the same as normal Hardcore mode but with all skills locked and alt-magic disabled. Does not affect existing characters, but one can use the Save Game Converter mod to change their gamemode (https://mod.io/g/melvoridle/m/save-game-converter) to convert existing HCs to "official" HCCO.

- No cap on bank slots. This is managed through a separate mod (https://mod.io/g/melvoridle/m/bank-space-manager) 

- Hardcore version has permadeath

- Mediumcore version has no permadeath

- No health regen

- Both have Hardcore/Adventure combat triangle (harsher penalties for using the wrong style)

Note: Uninstalling this mod will render any HCCO/MCCO account unplayable, similar to the official speedrun gamemodes after the expiration date (that is, they will still exist but won't be playable). Reinstall this mod and use the Save Game Converter mod if you want to continue playing any CO account as another gamemode.

Known issues and bug reporting
No known issues. Horray!

If you have any issues with the mod, feel free to message me on Discord directly (username: zxv) or post in the #hardcore-mode-chat in the official discord that has been co-opted by HCCO.

Posting a comment on this mod is also fine, but mod.io isn't terribly reliable at notifying me for new comments or replies so that will be slower.

Rebalance Mod Changes

Below is a reverse chronological list of the optional changes made with the various toggles in the mod, with the main one being the Rebalance toggle. The majority of the changes were made in V2.0, so scroll down to the bottom of the list to see the bulk of the gameplay changes implemented.

A complete list of drop table changes are available in game by clicking the "HCCO/MCCO Mod Vx.y" button in game under the regular game patch notes. This list is programmatically generated and will always be completely up to date.

V3.2 ACTUAL AOD PATCH HORRAY
AoD combat areas, slayer areas and dungeons are accessible through items obtainable through combat
Revamped entire drop table modification system
Bit technical, but "empty drops" are now no longer handled through the monster.lootChance variable. Every drop table now has an "empty drop" (signified by the empty equipment item), and any previous lootChance is converted directly to the weight of the empty drop item. This is a much more extensible system, and will make future drop table modifications much, much easier.
Drops added to tables first consume empty slots, then if there are no empty slots, now reduce the likelihood of *all* other items (by increasing the total weight of the drop table), instead of reducing the drop rate of a particular item. A few rare items (Ethereal weapons, Heated 2H Fury Hammer, Allure Amulet) have had their drop rates additionally tweaked to counteract this effect, so that their drop rate is similar (or the same) as live.
Added tortoise familiar.
Completion messages are now completely disabled, as they were firing at very inconvenient times. Hopefully these can be fixed in future to behave appropriately.
Updated in game patch notes generator. Monster drop changes are now displayed in a table format.
Added an optional, revamped display format which incorporates drop percentages, drop table weighting and minimum rolls.
V3.1
Updated some backend code to make the mode compatible with the new "No Resupply" mode: https://mod.io/g/melvoridle/m/no-resupply-hcco
Hardcore character Steam achievements can now be obtained on HCCO characters (not MCCO).
V3.0
AoD patch: updated some backend code to make the game compatible with the AoD expansion.
V2.38
Changed backend code to help with inter-mod compatibility. Specifically, progressmaps are now identified by the mod's namespace instead of a custom string that I plucked out of thin air.
V2.37
Added a new item log filtering option: "show ignored". This filter displays only items that are deliberately hidden from completion.
Non-CO items will no longer appear in the completion log search.
Added items from Township tasks to the completion log if Township tasks are enabled. 
V2.36
Fixed bug with items not being loaded correction on account creation.
V2.35
Fixed a bug where summoning tablets could be created directly.
V2.34
Completion Log bug fixes:
Removed mastery completely from the calculation of progress. This was causing brand new accounts to start with 20% completion due to mastery not being included. The game still doesn't calculate total completion percentage correctly, but at least now it's consistent.
Some items were incorrectly removed from the completion log. Specifically, many chests and their contents, items from IDE and anything with a slayer task requirement.
Fixed a bug where all completion log categories were double-counting CO items and had hugely inflated totals.
By fixing the above issue, the Combat Only completion percentage no longer changes when swapping between CO completion mode and full game completion mode.
Any Golbin Raid pets owned now show up in Combat Only selection.
V2.33
Split Rebalance option into two separate options. One option handles QoL fixes (e.g. removal of unobtainable shop items) and the other handles drop table and other gameplay changes.
Palladium bar drop from 50-150 to 100-200 to make grinding Divine (P) less painful
V2.32
Fixed bug where runepacks were not appearing in the shop.
V2.31
Totally revamped and updated the completion log backend. Should now filter inaccessible areas (e.g. Foggy Lake with no Rebalance mod) and associated items. Should also be completely compatible with future expansions.
V2.30
Fixed some menu translation issues.
V2.29
Disabled the item rebalance changes (FrostSpark Amulet, Leviathan Shield and Bundled Protection Body) as the game is refactoring the backend code and breaking these items.
V2.28
 I forgot to write down what I changed here, so no idea what happened in this patch!
V2.27
Dying no longer disables prayers, and HP is set to 60% after death instead of 20%.
V2.26
More bug fixes. Fixed issue with passive Township XP and pet gain. Both of these have now been disabled and any XP/pets obtained will be removed from everyone's account.
V2.25
Fixed compatibility issues with update.
V2.24
Restructured some internal code, so possible bugs may have been introduced.
Added Township tasks.
V2.23
Hide non-combat synergies
V2.22
Increased master wizard max quantity to 15 instead of 10 (as this was an unintentional nerf).
Fixed an issue with Siren drop table
V2.21
Fixed error in prayer and superior prayer cape shop descriptions.
V2.20
Partially fixed an issue with quick-equip and synergy menu equipping multiple tablets at max mark level. Unmaxed familiars can be equipped twice to equip the whole stack.
Plague Doctor drop rates increased from 1-2 to 1-5
RaZu lightning rune drop increased from 800 to 1500
Cockatrice decay bolts drop increased from 10-25 to 25-100
Dark Wizard drop table adjusted
Enchanted shield drop rate decreased from 20/379 to 15/379
Chaos rune drop quantity increased from 1-10 to 15-40
Death rune drop quantity increased from 1-10 to 15-40
Wizard scroll added to drop table at a rate of 5/379 with a drop quantity of 1000-1500
Priest drop table adjusted
Light rune drop rate decreased from 150/151 to 145/151
Prayer scroll added to drop table at a rate of 5/151 and a drop quantity of 1000-1500
V2.19
Fixed issue with divine platebody not appearing on Gret-Yun drop table.
Increased combat max cape offensive stats to match max cape.
V2.18
Fixed an issue where archaic runes weren't appearing on Frost Golem drop table.
Added experimental support for HCCO speedrun mode.
V2.17
Gret-Yun
Infernal rune drop rate increased from 55/120 to 56/120
Dragon bone drop rate reduced from 60/120 to 59/120
Changed positional reference to a proper reference for completion log HTML elements, fixing an issue with other mods that add items to the sidebar (e.g. Handy Dandy Notebook).
V2.16
Added automatically generated patch notes which displays all currently enabled drop table changes. Click the "HCCO/MCCO Mod Vx.y" button under the game version.
V2.15
Added a few missing items to the completion log:
Skilling gloves
Upgraded slayer items
Signet half ring (b)
Various non-dungeon chest items (e.g. Rubber ducky)
Added cooked shrimp to the Golbin drop table in the Rebalance at a rate of 1/27 and raw shrimp drop rate reduced from 6/27 to 5/27. This adds shrimp to the completion log but also ensures that accounts that transfer and people who created accounts before shrimp were added to the list of starter items can obtain shrimp and complete the completion log.
Redistributed divine drops from Burning Snake to all monsters in Lava Lake. The following changes are relative to the rebalanced gamemode.
Burning Snake
Chilli seed drop rate increased from 85/101 to 96/101
Divine helmet drop rate increased from 0 to 4/101
Divine boots drop rate reduced to 0
Divine shield drop rate reduced to 0
Divine platelegs drop rate reduced to 0
Divine platebody drop rate reduced to 0
Infernal Golem
Iridium ore drop rate reduced from 15/200 to 7/200
Divine boots drop rate increased from 0 to 8/200.
Magic Fire Demon
Fire rune drop rate reduced from 150/200 to 148/200
Infernal rune drop rate reduced from 49/200 to 48/200
Divine shield drop rate increased from 0 to 3/200
Manticore
Palladium ore drop rate reduced from 116/120 to 115/120
Divine platelegs drop rate increased from 0 to 1/120
Gret-Yun
Infernal rune drop rate reduced from 56/120 to 55/120
Divine platebody drop rate increased from 0 to 1/120
Priest light rune drop quantity increased from 1-10 to 10-30.
V2.14
Fixed issue with upgraded items not appearing in completion log.
(Hopefully) fixed issue with Summoning on Steam.
V2.13
Added some clarifying text inside the mod to help explain some of the mod features. The text on each of the mod buttons should explain what each setting does much better now.
V2.12
Fixed graphical issue with tablet quantity display when switching equipment sets.
Fixed graphical mark rebalance issue caused by loading with the feature disabled.
V2.11
Finally fixed the dodgy Summoning progress bar. Now the percentage properly tracks your progress through the level and the progress bar even has a tooltip.
Fixed an issue where rebalance item modifier patch was being applied even when the rebalance patch was disabled.
V2.10
If mark rebalance is enabled, marks can now only be obtained while the corresponding familiar is equipped.
Mark level 7 requirement reduced from 151 to 121 marks.
Fixed a bug where Max Cape variants were being loaded into the game after save files were read, causing the game to delete them on game load as they weren't registered yet. Sorry about that! If you were affected, contact me and I can refund the GP to your account.
V2.9
Fixed infernal golem drop table. Added iridium bars back in and appropriately reduced iridium ore drop rate.
Changed repeat slayer to a radio group, making the slayer options mutually exclusive.
Changed backend code so custom items are only loaded for CO characters.
Skilling summoning familiars have now been removed from the summoning interface.
Added optional rebalance for summoning mark mechanics. If enabled, the following two modifications to marks and familiars are applied:
Tablets for max level familiars will no longer be consumed.
Max level for familiars increased from 6 to 7, requiring 151 total marks to reach (90 more than level 6).

TODO:

Stop quick equip from equipping multiple familiars when mark level maxed out.
V2.8
Repeat current slayer task now incurs a -65% exp penalty as well.
Added missing ammo preservation back onto Combat Superior Max Cape
V2.7
Changed the passive effect on Bundled Protection Body, FrostSpark Amulet and Leviathan Shield to make these items more reliable. The goal is to eliminate the small chance of dying while the item effects are ramping up.
Bundled protection body passive changed. The old passive was removed and it now has the following two passives:
When stunned by an Enemy, heal for 12% of your max HP. Activates once per fight.
When stunned by an Enemy, gain +5% DR for the remainder of the fight. Activates once per fight.
FrostSpark amulet passive updated. In addition to the existing effect, now heals for 7% of your max HP on activation.
Leviathan Shield passive updated. In addition to the existing effect, when hit by an enemy, heal for 12% of your max HP and heal for 12% of your max HP when combat ends. Activates up to 5 times per fight.
Fixed issue with hitpoints cap not correctly applying (AGAIN).
V2.6
Fixed issue with hitpoints cap not correctly applying on load.
Fixed issue with combat max cape requiring summoning on load, causing equipped capes to be removed if Summoning wasn't enabled.
Added bronze dagger and 10 shrimp to the list of starting items.
V2.5
Fixed issue with certain modded drop tables crashing the game / bricking saves.
V2.4
Fixed issue where certain items were added to drop tables twice.
V2.3
Mark is now obtainable as a pet.
Fixed an issue with slayer coin penalty for repeat slayer task feature was being applied twice.
V2.2
This version now requires TotH. Please use https://mod.io/g/melvoridle/m/legacy-hcco if you do not have TotH.
Support for limited bank space has now been removed. Please use https://mod.io/g/melvoridle/m/bank-space-manager instead, as that mod handles the feature much better.
V2.1
Various bug fixes.
Added Golden Golbin to pet completion log.
Fixed HTML element load ordering issue (affected Repeat Slayer Button and Summoning Progress Tracker primarily).
V2.0
CO Rebalance Patch. That's right, we skipped straight over V1.0.

This patch brings a huge, optional rebalance to the CO gamemode. This rebalance was inspired due to the fact that a rather sizeable portion of vanilla end game is inaccessible or impossible on a CO. Foggy Lake was inaccessible due to having no way to obtain the required items for access. Enemies in Golden Cloud Mountains were simply too strong to kill with limited CO arsenal, and the two areas locked behind GCM were thus inaccessible. In addition, no archaic magick spells was usable due to no archaic rune source in the entire game, making magic considerably worse than the power level the game is balanced around.

This rebalance aims to rectify the above outlined issues and to also address the longstanding issue of magic requiring disproportionately more time to upkeep than the other two combat styles. The main method used to accomplish these goals are:

Added the items required to access Foggy Lake to various drop tables.
Added summoning as an optional skill that is designed with CO experience in mind
Rebalanced various drop tables to increase rune gathering speed
Added at least one source for every rune via a drop table.

Out of the support skills forfeited by CO accounts (Herblore, Summoning, Agility and Astrology), Summoning felt like the one that could be implemented in the most fitting way and would help to bridge the immense DPS and defence gap between CO and standard accounts. In RuneScape, Summoning is a combat skill already, and half of the skill in Melvor pertains to combat-isolated buffs. It is also possible to implement Summoning in a purely Combat way (by adding familiars to drop tables) and so the skill was a natural next fit out of the four (herblore has already been partially implemented with various potion drops being added in TotH).

At the moment, Archaic Magicks and Summoning are considered to be the minimal set of inclusions that have been added to hopefully make the end game richer. If necessary, more additions will be explored in future (most likely more herblore potions). Agility and astrology are unlikely to ever be added, but it remains to be seen if the game is beatable without those support skills.

In addition, this release also launches the CO Completion log. Filter out all inaccessible items, pets and skills and track your progress towards CO completion!

Please note that the rebalance and summoning addition are both optional, meaning you can opt to exclude them for a purely vanilla CO experience. Or you can go buck-wild and run multiple accounts; the choice is yours.

Unfortunately, there are some issues with the Steam version and this mod. HTML elements are loaded in a different order compared to browser and mobile, so some features aren't fully functional. This notably affects the repeat slayer button, completion log and skill progress bar. A fix is still being worked on.

V2.0 Patch Notes
External Mod Interactions
The following mods have been natively incorporated into this release. They are compatible with existing versions, and as they will only affect HCCO and MCCO characters it is recommended to keep the other mods installed for other gamemodes if desired.
Mini Max Capes (partially, only combat capes incorporated)
Slayer Reroll Fix
Repeat Current Slayer Task
Shop Requirements Lifter
Miscellaneous Changes
All food now heals for a minimum of 1 (no more AE1 Arid Plains horror stories).
An optional cap on bank space akin to vanilla hardcore mode has been added.
The ability to repeat slayer tasks has been added. This comes with a -65% multiplicative slayer coin penalty. This should make farming slayer tasks for task requirements much less painful, but it won't be better slayer coin income than variety slayer.
Resupplies and packs can now be purchased with limited bank space as long as the player has enough items already in their bank from the purchase. Previously the player needed to have every item or more than 5 bank spaces open in order to purchase resupplies. Now, for example, a pack can be bought with 1 empty bank space if the player owns 4 out of the 5 items given by the pack.
Summoning has been added as an optional combat skill. Tablets cannot be created directly, but tablets have been added to various monster and dungeon drop tables. Marks still need to be obtained as a drop at least once before additional marks can be obtained.
If enabled, summoning now contributes to combat level in the same manner as prayer.
If enabled, a summoning requirement has been added to the combat max cape and superior version.
If summoning is enabled, the combat max cape now has a 10% chance to preserve summoning charges.
If summoning is enabled, the combat superior max cape now has a 15% chance to preserve summoning charges.
Drop Table Adjustments
Several monsters have had their drop tables rebalanced. The overall goal was to make magic much less painful by making the rune gathering process easier, and to add sources of familiars for the summoning skill. This is still being balanced and will be revisited in future if necessary.
The following have had quantity adjustments (drop rates unchanged)

Magic Chest:
Air, water, earth and fire now a drop quantity of 400-800, up from 1-100
Chaos and death runes now have a drop quantity of 400-800, up from 1-50
Ancient runes now have a drop quantity of 500-1500, up from 1-10
Water Chest:
Death, blood and ancient runes now have a drop quantity of 500-1000, up from 1-1000
Wizards:
Air, water, earth, fire runes now have a drop quantity of 10-30, up from 1-10
Master Wizards:
Mind runes now have a drop quantity of 5-10. Up from 1-10
Magic Fire Demon:
Fire runes now have a drop quantity of 10-30, up from 1-10
Lava runes now have a drop quantity of 50-100, up from 1-10
Gret-Yun:
Infernal runes now have a drop quantity of 20-50, up from 1-20
Ice Hydra:
Calamity runes now have a drop quantity of 100-200, up from 1-20
Siren:
Despair runes now have a drop quantity of 15-30, up from 1-15
Polar bear:
Frost crabs now have a drop quantity of 50-80, up from 1-3
Frozen manta rays now have a drop quantity of 150-300, up from 1-3
Cockatrice:
Decay bolts now have a drop quantity of 10-25, up from 1-10
Plague doctor:
Hinder potion III, lethal toxins potion III, area control potion III, reaper potion III, famished potion III and penetration potion III now have a drop quantity of 1-2, up from 1-1
The following have had drop rates adjusted and new items added to fill the gaps. Drop rate adjustments to make room for summoning tablets are only when the skill is enabled.

Miolite Chest:
Miolite boots drop rate has been reduced from 100/199 to 53/199
Miolite helmet drop rate has been reduced from 50/199 to 27/199
Miolite shield drop rate has been reduced from 20/199 to 13/99
Miolite spore drop rate has been reduced from 13/199 to 7/199
Miolite platelegs drop rate has been reduced from 10/199 to 5/199
Miolite platebody drop rate has been reduced from 5/199 to 3/199
Mist, dust and mud runes have had their drop rate increased from 0 to 20/199, with a drop quantity of 200-400
Smoke, steam and lava runes drop rates have increased from 0 to 10/199, with a drop quantity of 200-400
Ancient Chest:
Carrion bark drop rate has been reduced from 60/133 to 46/133.
Jungle spores drop rate has been reduced from 30/133 to 25/133.
Linden log drop rate increased from 0 to 19/133, with a drop quantity of 150-300.
Burning chest:
infernal bones drop rate has been reduced from 30/82 to 20/82
Ash drop rate has been reduced from 20/82 to 14/82
Charcoal drop rate has been reduced from 20/82 to 14/82
Palladium bar drop rate has increased from 0 to 22/82, with a drop quantity of 50-150
Lightning Region:
Lightning spirit now drops 51 lightning spirit tablets
Lightning monkey now drops 53 lightning spirit tablets
Lightning golem now drops 58 lightning spirit tablets
RaZu now drops 800 lightning runes
Lair of the Spider Queen:
Each random spider now drops 53 spider tablets.
Spider Queen now drops 350 spider tablets.
Necromancer's Palace:
Cursed Skeleton Warrior now drops 120 lightning spirit tablets
Beholder now drops 150 siren tablets
Dark knight now drops 200 spider tablets.
Fiozor now drops 600 spectre tablets.
Lots of Eyes:
Eyeball drop rate reduced from 5/6 to 3/6
Golbin theif tablet drop rate increased from 0 to 2/6
Many Eyed Monster:
Eyeball drop rate reduced from 5/6 to 1/6
Wolf and occultist tablet drop rates increased from 0 to 2/6
Strange Eyed Monster:
Eyeball drop rate reduced from 5/6 to 1/6
Witch and minotaur tablet drop rates increased from 0 to 2/6
Eyes:
Eyeball drop rate reduced from 5/6 to 1/6
Cyclops and centaur drop rate increased from 0 to 2/6
Superior Eyed Monster:
Eyeball drop rate reduced from 5/6 to 1/6
Yak and unicorn drop rate increased from 0 to 2/6
Eye of Fear:
Eyeball drop rate reduced from 5/6 to 3/6
Dragon tablet drop rate increased from 0 to 2/6
Poison Toad:
Bitterlyme seed drop rate increased from 10/700 to 496/700
Poison rune drop rate increased from 0 to 200/700
All empty drops have been removed and mostly replaced with Bitterlyme seeds.
Burning Snake:
Chilli seed drop rate decreased from 100/202 to 85/202
Divine helmet and divine boots drop rate increased from 0 to 4/202, with a drop quantity of 1-1
Divine shield drop rate increased from 0 to 3/202, with a drop quantity of 1-1
Divine platelegs and divine platebody drop rate increased from 0 to 2/202, with a drop quantity of 1-1
Infernal Golem:
Iridium ore drop rate reduced from 65/200 to 15/200
Iridium bar drop rate increased from 0 to 50/200, with a drop quantity of 10-25
Lava rune drop rate quantity increased to 25-35, up from 1-10
Frost Golem:
Water rune drop rate decreased from 149/150 to 100/150, with a drop quantity of 35-80
Archaic rune drop rate increased from 0 to 49/150, with a drop quantity of 35-80
Valkyrie:
Absorbing shield drop rate increased from 0 to 1/200
Spectre, Banshee and Phantom:
Moonwort drop rate reduced from 500/501 to 300/501 (no summoning) or 100/501 (with summoning)
Soul rune and spectre tablet drop rate increased from 0 to 200/501, with a drop quantity of 250-500.
Siren:
Despair rune now have a drop quantity of 15-30, up from 1-15. If summoning is enabled, despair rune drop rate reduced from 277/290 to 139/290 and drop quantity increased to 30-60
If summoning is enabled, siren tablet drop rate increased from 0 to 138/290
Shop Changes
Light runes have been removed from slayer resupplies.
Cooking Upgrade 2 has had its cooking requirement removed. The gold price remains unchanged.
Items that cannot be purchased due to CO restrictions have been removed from the shop.
Four tiers of runepack have been added to the slayer shop.
Apprentice runepack. Costs 15k slayer coins and contains 250 of the following runes: air, water, earth, fire, light, body, mind and chaos runes
Adept runepack. Costs 30k slayer coins and contains 350 of the following runes: mist, dust, smoke, nature, havoc and death runes
Master runepack. Costs 60k slayer coins and contains 450 of the following runes: steam, mud, lava, spirit, blood and ancient runes
Archmage runepack. Costs 120k slayer coins and contains 550 of the following runes: poison, infernal, lightning, decay, soul, despair, archaic and calamity runes
Four tiers of summoning tablet packs have been added to the slayer shop.
Critter pack. Costs 15k slayer coins and contains 250 of the following familiars: golbin thief, occultist and wolf familiars
Companion pack. Costs 30k slayer coins and contains 350 of the following familiars: minotaur, witch, centaur and cyclops familiars
Familiar pack. Costs 60k slayer coins and contains 450 of the following familiars: yak, unicorn and dragon familiars
Beast pack. Costs 120k slayer coins and contains 550 of the following familiars: lightning spirit, siren, spider and spectre familiars
Nerfs
Hitpoints is now capped at 99 until after 10,000 combined Dark Waters monster kills. This was done to respect the extremely well balanced state the CO gamemode was inadvertently in before the expansion, while still making IDE much easier to complete than pre-expansion (as this was a pain point for a lot of players). XP is still gained beyond 99 when capped and the other combat skills are unaffected.
The following nerfs have been applied to the following items. The reasoning is that their effect was frankly too strong and completely trivialised prayer as a resource. It was relatively balanced pre-expansion due to cape slot being highly contested, but as the effect can now be readily obtained through the combat max capes it was simply too strong to leave unchanged.
The prayer skillcape and combat max skillcape now reduce prayer point costs by 25%, down from 50%.
The superior prayer skillcape and combat superior max skillcape now reduce prayer point costs by 35%, down from 75%.
TODO

While I am incredibly happy with the amount of content contained within this patch, there are still some outstanding additions that I would like to add to the mode in future. In particular:

Bug fix: prevent completion log popup from firing when changing visible display
A rework of bundled protection body, frostspark amulet and leviathan shield to be much more consistent. The aim is to prevent idle deaths while the items ramp up in power throughout the fight.
Add Mark as an obtainable pet for completing necessary mark tiers for combat familiars
Bug fix: Fix HTML issues with steam client
Visual bug fix: Fix issue where summoning requirement on pack is red until monster killed

----

[Just the Docs]: https://just-the-docs.github.io/just-the-docs/
[GitHub Pages]: https://docs.github.com/en/pages
[README]: https://github.com/just-the-docs/just-the-docs-template/blob/main/README.md
[Jekyll]: https://jekyllrb.com
[GitHub Pages / Actions workflow]: https://github.blog/changelog/2022-07-27-github-pages-custom-github-actions-workflows-beta/
[use this template]: https://github.com/just-the-docs/just-the-docs-template/generate
