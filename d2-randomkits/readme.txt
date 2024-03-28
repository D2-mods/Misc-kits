GitHub: https://github.com/D2-mods/Misc-kits

Notes:
- Compatible with EEs and classic BG2 engine
- Mod made with Notepad++, WeiDU, and Near Infinity
- Uses ADD_KIT_EX function by Argent77 (https://github.com/Argent77/A7-add_kit_ex)
- LibIconv (http://gnuwin32.sourceforge.net/packages/libiconv.htm)


//Kits
Kensaizerker (fighter)     - EE and classic
Monastery Swordsman (monk) - EE only
Jesterblade (bard)         - EE and classic

//config.ini
Set a kit to = 0 to prevent install


Translations:
- French (JohnBob)

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------

v2.7
- Monastery Swordsman: Sever now adds 9d6 slashing damage (previously 5d6). It no longer has a save penalty for the vorpal effect. It will now always play a visual effect on hit. Reordered effects so that the extra slashing damage is applied before vorpal hit (i.e. will always be shown in combat log). Sever is now gained at levels 13 and 17.
- Jesterblade: Song's save bonus now lowers by 1 every 5 levels, up to -2 at level 20. Confusion now lasts 10 seconds. Song effects are no longer dispelled each time song is played (EEs). Song now actually affects enemies within 30 feet (Jester song is only 15 feet, despite the description). Note that the song still does not gain the extra effects from the regular Jester song.
- Updated functions.
- Various installer improvements, mostly copied over from the Workshop Kitpack.

v2.6
- Monastery Swordsman compatibility fix: 
	- Fixed an APR issue if using subtledoctor's APR tweak (all classes get bonus APR from Specialization).
	- The fix doesn't depend on install order. This mod can/should still be installed before tweak mods.

v2.5
- Kits will now gain the bonus effects from certain Beamdog items:
	- Bartleby's Wakizashi: Kensaizerker, Monastery Swordsman
	- Belt of the Skillful Blade: Jesterblade
	- Dragon Blade: Kensaizerker (while enraged)
	- Screaming Bagpipes: Jesterblade

v2.4
- Fixed potential issues in classic BG2 (both Kensaizerker and Jesterblade).

v2.3
- Kensaizerker: Fixed an issue from the last update, which could cause this kit to fail to install.

v2.2
- Kensaizerker: 
	- EEs: Will use the vanilla Enrage if the Berserker rework from Artisan's kitpack is installed.
	- BGEE/IWDEE: Added fixes for potential issues with string immunities.

v2.1
- Monastery Swordsman: 
	- Installing this kit will now also re-enable the Monk class (if disabled by another mod).
	- Install after any mods that disable the Monk class (i.e. Monastic Orders v0.42).

v2.0
- Kit abilities are now unaffected by casting speed penalties.
- Fixed harmless WeiDU warning when installed after EE Fixpack.

v1.9
- Added French translation by 11jo

v1.8
- Jesterblade: fixed compatibility when installed after Rogue Rebalancing revisions
	- Works the same way as with Bardic Wonders. Song will be the vanilla Jester song. Everything else will be based on the revised Blade if installed.

v1.7
- Jesterblade: fixed compatibility when installed after Bardic Wonders revisions
	- will always use the vanilla Jester song (Confuse at +2 bonus)
	- if revised Blade is installed, everything else will be based on the Blade revision

v1.6
- all kits now clone an existing abilities table:
	- Kensaizerker clones the base Fighter table
	- Monastery Swordsman clones the base Monk table
	- Jesterblade clones the Blade table

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------

//Kit descriptions

==================================================
Kensaizerker (Fighter)
==================================================
KENSAIZERKER: A variant of the kensai, or "sword saint", this warrior is in tune with <PRO_HISHER> animalistic side and, during combat, can achieve an ecstatic state of mind that will enable <PRO_HIMHER> to fight longer, harder, and more savagely than any person has a right to.

Advantages:
– +2 bonus to Armor Class.
– +1 to attack and damage rolls every 3 levels.
– -1 bonus to Speed Factor every 4 levels.
– May use the Enrage ability. Gains one use at level 1 and an additional use every 4 levels thereafter.

ENRAGE: For 1 turn, the character gains a +2 bonus to attack and damage rolls, a +2 bonus to Armor Class, and immunity to charm, confusion, fear, feeblemind, hold, imprisonment, level drain, maze, stun, and sleep. The character also gains 15 temporary Hit Points which are taken away at the end of the berserk spree, possibly knocking <PRO_HIMHER> unconscious.

Disadvantages:
– Becomes winded after berserking: -2 penalty to attack rolls, damage, and Armor Class.
– May not wear any armor.
– May not use missile weapons.
– May not wear gauntlets or bracers.
– Alignment restricted to any non-lawful.


==================================================
Monastery Swordsman (Monk)
==================================================
MONASTERY SWORDSMAN: Monks are warriors who pursue perfection through contemplation as well as action. Among them are a subset that have been specially trained to be one with their favored weapons. This Monk's best known feat is the ability to sever an opponent with a single strike.

Advantages:
– May achieve High Mastery (four slots) in any weapon available to Monks.
– May place 2 slots in Single Weapon Style and 3 slots in Two-Weapon Style.
– +1 to attack and damage rolls every 4 levels.
– 2nd level: May use the Blazing Weapon ability once per day. Gains additional uses every 4 levels thereafter.

BLAZING WEAPON: Shrouds weapons in an intense, but short-lived, flame. Melee attacks deal an extra 2d6 fire damage per hit for the next round. The duration increases to 2 rounds at level 9, 3 rounds at level 12, 4 rounds at level 15, and 5 rounds at level 25.

– 13th level: May use the Sever ability once per day. Gains an additional use at level 17.

SEVER: A single deadly strike. On the next successful melee attack within 2 rounds, the target takes an extra 9d6 slashing damage and must save vs. Death or die.

Disadvantages:
– Unarmed attacks do not gain extra Attacks Per Round bonuses.
– May not use the Stunning Blow ability.
– May not use the Quivering Palm ability.
– May not use slings or darts.


==================================================
Jesterblade (Bard)
==================================================
JESTERBLADE: The Jesterblade is well versed in the arts of ridicule and hilarity, and uses <PRO_HISHER> abilities to confuse enemies, cavorting madly during combat. Do not mistake <PRO_HIMHER> for a true fool, however. This bard is an expert fighter and adventurer, whose fighting style is lethally dangerous.

Advantages:
– The Jesterblade's song confuses enemies within 30 feet unless they save vs. Spell at a +2 bonus. The bonus lowers to +1 at level 5, +0 at level 10, -1 at level 15, and -2 at level 20.
– May place 3 slots in Two-Weapon Style.
– May use the Offensive Spin and Defensive Spin abilities once per day. Gains one use each at level 1 and an additional use each every 4 levels thereafter.

OFFENSIVE SPIN: During the next 4 rounds, the character gains a +2 bonus to attack and damage rolls, an extra attack per round, and doubled movement speed. As well, all attacks do maximum damage for the duration. Offensive Spin may not be used in conjunction with the Haste or Improved Haste spells.

DEFENSIVE SPIN: During the next 4 rounds, the character is rooted to the spot and gains a +1 bonus to Armor Class per level, up to a maximum of +10.
  
Disadvantages:
– Bard Song does not gain additional effects at higher levels.
– Only has one half the normal Lore value.
– Only has one half the normal Pick Pockets skill.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------