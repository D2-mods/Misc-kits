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
- French (by 11jo)

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------

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
– May allocate two slots in Single Weapon Style and three slots in Two-Weapon Style.
– +1 to attack and damage rolls every 4 levels.
– 2nd level: May use the Blazing Weapon ability once per day. Gains additional uses every 4 levels thereafter.

BLAZING WEAPON: The monk channels inner light, shrouding weapons in an intense, but short-lived, flame. Melee attacks inflict an extra 2d6 fire damage per hit for the next round. The duration increases to 2 rounds at level 9, 3 rounds at level 12, 4 rounds at level 15, and 5 rounds at level 25.

– 13th level: May use the Sever ability once per day.

SEVER: A single deadly strike. The next successful attack within 2 rounds forces the target to save vs. Death at -2 or die. An opponent that survives the attack still suffers 5d6 slashing damage.

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
– The Jesterblade's song does not help allies. Instead, once each round, every enemy within 30 feet must save vs. Spell with a +2 bonus or be confused for 1 round.
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