GitHub: https://github.com/D2-mods/Misc-kits
Download: https://github.com/D2-mods/Misc-kits/releases
Languages: English, French (JohnBob)

--

Overview:
- Compatible with EEs and classic BG2 engine.
- Originally made as a practice mod to learn kit creation.
- Ability tables are made by cloning the table of the base class/kit.

v3.0 update:
- Monastery Swordsman changed to use Ki Energy system (also used by Medic from Workshop Kitpack).
- Added Kit Updater component. Run after all mods are installed (except possibly Dual to Kit).
- Compat improvements with tweak/overhaul mods (especially ToF, HLA mods, and proficiency mods).
- BG2 (classic): Added ranger variant of Monastery Swordsman.

--

Kits
- Kensaizerker (fighter)       - EE and classic
- Monastery Swordsman (monk)   - EE only
- Jesterblade (bard)           - EE and classic
- Monastery Swordsman (ranger) - alt kit for classic BG2

Components
1. Install kits
2. Choose Enrage version (options in installer)
3. Kit Updater (see below)

--

Install notes:
- config.ini: Set a kit to = 0 to prevent install
- Updater and Enrage components can be re-run at any time.
- Install after class revisions, except for Talents of Faerun. If another revision says to install after all kit mods, you can try it both ways.
- Safe to install before or after most tweak mods, including proficiency revisions. It's still recommended to follow normal install order guidelines.

Kit Updater:
- Updates HLA tables, Proficiencies, misc fixes, mod compat, etc.
- Monastery Swordsman: Can put max slots in any melee weapon usable by base Monk.
- Run after all tweak and overhaul mods, including mods that say to install last.
- Dual to Kit note: Run this once before Dual to Kit if using a proficiency tweak. It can be re-run after if you need to update other things later. (note: it's specifically component 3 of Dual to Kit that needs to be after any proficiency edits)

Talents of Faerun notes:
- Run the Updater after ToF. This is REQUIRED for compatibility.
- Jesterblade can select Blade-only abilities at same level as Blade. If ToF selectable songs are detected, the Jesterblade song will also have a song switching ability.
- Monastery Swordsman can learn some fighter abilities at same level as fighter. It has access to all fighter HLAs, in addition to most monk ones.

--

Translations:
- French (JohnBob)

Functions (not including my own):
- ADD_KIT_EX function by Argent77 (https://github.com/Argent77/A7-add_kit_ex)
- CD_EXTEND-O-MATIC function by CamDawg (https://www.gibberlings3.net/forums/topic/28835-toss-your-semi-useful-weidu-macros-here/page/13/#comment-332943)
- GET_KIT_STRREF (source unknown)

Older (v2.x) ki system:
- semi_innate_casting function by subtledoctor (https://github.com/subtledoctor/SD_useful_functions)

Tools:
- Mod made with Notepad++, WeiDU, and Near Infinity
- LibIconv (http://gnuwin32.sourceforge.net/packages/libiconv.htm)

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------

v3.0
- EEs: Changed Monastery Swordsman to use the Ki Energy system (also used by Medic from Workshop Kitpack). This is a regenerating ability points system. It works seamlessly with Bubb's Menu overlay mode (one of the main reasons I made my own system). See kit description. Ki/ability progression is different than with v2.x versions.
- BG2 (classic): Added Monastery Swordsman as a ranger kit (see kit description). It has all passive bonuses of the monk class, including mod revisions if made before this mod. Item restrictions are same as kensai (no bracers but can use the offhand, unlike monks in original BG2).
- BG2 (classic): Fixed issues with default Enrage option caused by recent effects structure changes. (Enrage was missing ability icon, Winded icon/text was not displaying)
- Tweaked visuals for Monastery Swordsman's Element weapon abilities. The wind and moon ones also play a visual on hit now, instead of looking like a normal hit. Wind hit is also delayed 1 second to time with visual.
- Kensaizerker: Winded/Rest fix for classic BG2 (this was already fixed for kit in EEs). If resting while Enrage is still active, the character no longer takes damage or becomes winded after Rest.
- Monastery Swordsman: Element abilities now also make the weapon glow a solid color (still has portrait icon). Also fixed some effects being dispellable.
- ToF mod: Fixed Option 2 of Enrage component being stackable with ToF (if using revised kits + feats components).
- Kensaizerker: if using any mod that adds an "Extra Enrage" HLA (ex. ToF), this will now give the correct spell resource, so you won't have 2 separate enrage icons in the special abilities menu. For ToF specifically, this adds a new HLA to m_dw_hld.lua instead of changing the berserker HLA (it won't appear for other kits).
- BG2 (classic): If Monastery Swordsman is installed, the Scarlet Ninjato item is usable by rangers. Can optionally make not usable by rangers from config.ini.
- BG2 (classic): Fixed installer error if you didn't have TobEx installed. It was scanning a file that I didn't realize was added by TobEx and not in the base game.

v2.16
- Kit Updater: Fixed issue where the updater was removing tweaks to the Jesterblade's clab/abilities table. Now, anything not accounted for is left untouched by the updater.
- Jesterblade: Jesterblade can now take Whirlwind HLA with or without bard revisions. It will now always have access to HLA traps, even if a revision removed them (ex. ToF or Rogue Rebalancing).
- Monastery Swordsman: Installer now checks for some fist-only HLAs added by mods (ex. Artisan's Kitpack). These will be removed for this kit. Instead, it will gain equivalent fighter hlas.
- Fixed Monastery Swordsman not being able to use Big Metal Rod (every class/kit can use this).
- Compat fixes with Shohy's bard mod (hide 2 weapon prof, fixed Lingering Song HLA being unselectable).

v2.15
Talents of Faerun notes:
- Kit Updater now does some specific ToF patching. Updates HLA lists, mod compat for Jesterblade, and proficiencies for Monastery Swordsman. Run the Kit Updater any time after ToF to update.
- Jesterblade can now select Blade-only abilities at same level as Blade. It can also now select IWD songs (similar to Blade and Jester kits).
- if ToF selectable songs are detected, the Jesterblade's song will also give an ability to switch to it. Selectable songs are added if you install IWD songs + minor/high level abilities.
- Monastery Swordsman can now learn Improved Criticals and Dirty Fighting at same level as fighter.

v2.14
- Changed "Update HLAs" component to "Kit Updater". It now also updates the Monastery Swordsman's HLAs and proficiencies if relevant tweaks were installed after this mod. This component can be re-run at any time.
- Monastery Swordsman can now be installed before or after Monk usability tweaks and proficiency overhauls (except for Talents of Faerun overhaul). Any melee weapon or fighting style that the base monk has access to will be set to max ("max" being whatever the base fighter class is set to).
- ToF note: Monastery Swordsman can gain grandmastery in all melee weapons with the ToF overhaul. The overhaul does this part by itself (the updater isn't needed specifically for this).
- Fix ids warning when installing on original BG2 engine (this was harmless, but annoying to see).
- EEs: Monastery Swordsman is now listed in the "Not Usably By:" part of the item description for slings and darts.
- Kensizerker: Improved effects structure for Enrage ability.
- Enrage component is now skipped if kensaizerker is not installed.

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
– May achieve Grand Mastery (five slots) in any melee weapon available to Monks.
– May place 2 slots in Single Weapon Style and 3 slots in Two-Weapon Style.
– +1 to attack and damage rolls at 3rd level and an additional +1 bonus every 5 levels thereafter.
– Gains Ki Energy, which is used to activate kit abilities. Gains +1 per level to maximum Ki Energy, up to level 20.
– Ki Regen: The character passively regains +1 Ki Energy every 5 rounds.
– 3rd level: May use the Element—Fire ability. Requires 3 Ki Energy.

ELEMENT—FIRE: For 4 rounds, each successful melee attack deals an extra 2d6 fire damage.

– 5th level: May use the Element—Wind ability. Requires 3 Ki Energy.

ELEMENT—WIND: For 4 rounds, each successful melee attack deals an extra 2d6 slashing damage.

– 7th level: May use the Element—Moon ability. Requires 3 Ki Energy.

ELEMENT—MOON: For 4 rounds, each successful melee attack deals an extra 2d6 magic damage.

– 13th level: May use the Sever ability. Requires 6 Ki Energy.

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

//alt kit for classic BG2

==================================================
Monastery Swordsman (Ranger)
==================================================
MONASTERY SWORDSMAN: These finely skilled warriors channel a subtle energy, called ki, to perform amazing feats. Their best known feat is the ability to sever an opponent with a single strike.

Advantages:
-  Gains all passive bonuses of the monk class, except for improved fist attacks.
-  May achieve Grand Mastery in any melee weapon that a thief can use.
-  Bonus +1 to hit and +1 to damage at 3rd level and every 5 levels thereafter.
-  3rd level:  May use the Element—Fire ability once per day. Gains additional uses at levels 8 and 20.

ELEMENT—FIRE: For 4 rounds, each successful melee attack deals an extra 2d6 fire damage.

-  6th level:  May use the Element—Wind ability once per day. Gains additional uses at levels 11 and 20.

ELEMENT—WIND: For 4 rounds, each successful melee attack deals an extra 2d6 slashing damage.

-  7th level:  Lay on Hands to heal 2 hit points per level
-  9th level:  May use the Element—Moon ability once per day. Gains additional uses at levels 14 and 20.

ELEMENT—MOON: For 4 rounds, each successful melee attack deals an extra 2d6 magic damage.

-  13th level:  May use the Sever ability once per day. Gains an additional use at level 18.

SEVER: A single deadly strike. The next successful attack within 1 round forces the target to make a save vs. Death at -2 or die. An opponent that survives the attack still suffers 5d6 slashing damage.

Disadvantages:
-  May not use missile weapons
-  May not wear armor or helmets
-  May not wear gauntlets or bracers
-  May not use shields
-  May not use 'charm animal' ability
-  May not cast priest spells
-  Cannot be chaotic alignments

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------