GitHub: https://github.com/D2-mods/Misc-kits

Notes:
- Compatible with EEs and classic BG2 engine
- Uses ADD_KIT_EX function by Argent77 (https://github.com/Argent77/A7-add_kit_ex)
- Uses semi_innate_casting function by subtledoctor (https://github.com/subtledoctor/SD_useful_functions)
- Uses CD_EXTEND-O-MATIC function by CamDawg (https://www.gibberlings3.net/forums/topic/28835-toss-your-semi-useful-weidu-macros-here/page/13/#comment-332943)

--

Kits
- Kensaizerker (fighter)     - EE and classic
- Monastery Swordsman (monk) - EE only
- Jesterblade (bard)         - EE and classic

Components
1. Install kits
2. Choose Enrage version (options in installer)
3. Update HLAs (only relevant if HLAs were revised)

--

Notes:
- config.ini: Set a kit to = 0 to prevent install
- Update HLAs: safe to install after Talents of Faerun. ToF "minor abilities" that require a level check for Blade are not selectable by Jesterblade. One of these, Ambidexterity, will be given to the Jesterblade for free at level 20.

Translations:
- French (JohnBob)

Tools:
- Mod made with Notepad++, WeiDU, and Near Infinity
- LibIconv (http://gnuwin32.sourceforge.net/packages/libiconv.htm)

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------

v2.13
- updated French translation from JohnBob.
- made installer options for Enrage component more descriptive.
- EEs: fixed bug where character is winded if party Rests while Enrage is still active (both Enrage options).
- IWDEE: kensaizerker Enrage no longer prevents resting in IWDEE (both Enrage options). This was probably meant to be a fix for being winded after Rest (only Berserkers are prevented from resting, not Barbarians). Since I fixed the real issue, it isn't necessary for this kit.
- added support for EE fixpack status immunity spellstates.
- re-up of v2.13: fixed v2.13 mistake that made Jesterblade learn regular Jester song at level 20.
- fixed oversight that could cause installer to leave leftover files in the override after uninstall.
- fixed possible issue of duplicated text, if running the "update HLAs" component multiple times in a row.

v2.12
- Kensaizerker: fixed Enrage being stackable with Option 2 of Enrage component.
- Kensaizerker: now uses the Berserker HLA table as base if modded (previously using Kensai table).
- Jesterblade: now compatible with Bardic Wonders song mechanics tweak. Must be installed after Bardic Wonders. A note is added to bottom of kit description with tweak info.
- Jesterblade: now compatible with IWDification "Selectable Bard Songs" tweak (both EE and classic). Must be installed after IWDification. The Jesterblade song change ability is made by cloning the Jester one from IWDification.
- Added component: Update HLAs for Kensaizerker and Jesterblade. Use if HLA lists were changed after this mod was installed. It might do nothing, or it might do something (depends on what mod HLAs are detected). This is safe to run after ToF.
- various other mod compat work. Note that Kensaizerker and Jesterblade internally are considered Kensai and Blade for item restrictions (if a mod adds kit-specific items).

v2.11
- Jesterblade:
	- fixed compat with Bardic Wonders if installed song mechanics tweak without Jester revision before this mod.
	- improved song install, which should avoid most compatibility issues (even with mods I haven't tested with).

v2.10
Jesterblade - Compat notes:
- Rogue Rebalancing:
	- Jesterblade will now gain the passive bonuses from both Blade and Jester. Must be installed after rr.
	- HLA list uses the Blade list, with Jester HLA Song added. Must be installed after rr.
- Shohy's bard song mod:
	- Fixed an issue where Jesterblade was gaining regular bard songs if this mod was installed after Shohy's mod.
	- Jesterblade will gain the passive bonuses from both Blade and Jester. Must be installed after Shohy's mod.
	- HLA list uses the Blade list, with song replaced by Jester HLA Song. Must be installed after Shohy's mod. If selected, will also gain the "chorus" abilities. The chorus abilities are not gained naturally as they have no effect on the normal Jesterblade song.
- Bardic Wonders:
	- Jesterblade will gain all Blade revision stuff, except for the Blade song. Must be installed after Bardic Wonders.
	- Jesterblade will now gain the Heckle ability if Jester revision is installed. Must be installed after Bardic Wonders.
	- HLA list is identical to the Blade list (no song added, Jester HLA song is too different from the Jesterblade song).

Kensaizerker - Compat notes:
	- Artisan's kitpack: no longer gains Rapid Shot when installed after fighter revision. It will gain the melee abilities. It does not gain passives from Berserker or Kensai revisions (balanced too different from the unmodded kits).
	- Added component "Choose Enrage version". Can set the kit's Enrage to a custom spell that always has vanilla effects (default), or set to the base game Enrage, including possible tweaks (ex. from ToF). This component can be re-run at any time to change setting, and works with existing save games (will update any Enrages already gained).


v2.8
- Monastery Swordsman update:
	- It now uses the ability pool system by subtledoctor (lore-wise called "ki points"). It now gains 3 elemental weapon abilities at level 3 (Fire, Wind, Moon). It still gains Sever at level 13, but now as part of the same points pool as other abilities.
	- Sever is reverted back to the pre-v2.7 version (5d6 damage, save at -2 or die). Vorpal effect now uses the chunked death animation (does not destroy items). Changed the vorpal hit visual to the same one used in IWDEE for the Solemn Duty katana.
	- Can now reach Grand mastery in weapons.
	- Slightly nerfed bonus to hit/damage. It now starts at level 3, and every 5 levels after (3, 8, 13, 18, etc.).

v2.7
- Monastery Swordsman: Sever damage increased from 5d6 to 9d6. It no longer has a save penalty for the vorpal effect. It will now always play a visual effect on hit. Reordered effects so that the extra slashing damage is applied before vorpal hit (i.e. will always be shown in combat log). Sever is now gained at levels 13 and 17.
- Jesterblade: Song's save bonus now starts at +2 and lowers by 1 every 5 levels, up to -2 at level 20. Confusion now lasts 10 seconds. Song effects are no longer dispelled each time song is played (EEs). Song now affects all enemies in visual range (was previously fireball range). Note that the song still does not gain the extra effects from the regular Jester song.
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
– May achieve Grand Mastery (five slots) in any weapon available to Monks.
– May place 2 slots in Single Weapon Style and 3 slots in Two-Weapon Style.
– +1 to attack and damage rolls at 3rd level and an additional +1 bonus every 5 levels thereafter.
– Gains ki points, which are used to activate kit abilities. Gains 1 ki point every 3 levels, up to a maximum of 10 points at level 30.
– 3rd level: May use the Element—Fire, Element—Wind, and Element—Moon abilities. Each requires 1 ki point.

ELEMENT—FIRE/WIND/MOON: For 4 rounds, each successful melee attack deals an extra 2d6 fire, slashing, or magic damage. Only one element can be in effect at a time.

– 13th level: May use the Sever ability. Requires 1 ki point.

SEVER: A single deadly strike. The next successful attack within 2 rounds forces the target to make a save vs. Death at -2 or die. An opponent that survives the attack still suffers 5d6 slashing damage.

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

OFFENSIVE SPIN: During the next 4 rounds, the character gains a +2 bonus to attack and damage rolls, an extra attack per round, doubled movement rate, and all attacks deal maximum damage for the duration. Offensive Spin may not be used in conjunction with the Haste or Improved Haste spells.

DEFENSIVE SPIN: During the next 4 rounds, the character is rooted to the spot and gains a +1 bonus to Armor Class per level, up to a maximum of +10.
  
Disadvantages:
– Bard Song does not gain additional effects at higher levels.
– Only has one half the normal Lore value.
– Only has one half the normal Pick Pockets skill.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------