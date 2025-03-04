# Misc kits

Download: https://github.com/D2-mods/Misc-kits/releases  
Languages: English, French (JohnBob)

Some kits I made for practice, while planning a bigger kitpack -> [The Workshop Kitpack](https://github.com/D2-mods/The-Workshop-Kitpack).

#### Notes:
- compatible with EEs and classic BG2 engine
- uses ADD_KIT_EX function by Argent77 (https://github.com/Argent77/A7-add_kit_ex)

--

### Kits
<details>
  <summary>Kensaizerker (fighter)     - EE and classic</summary>
  
---

KENSAIZERKER: A variant of the kensai, or "sword saint", this warrior is in tune with <PRO_HISHER> animalistic side and, during combat, can achieve an ecstatic state of mind that will enable <PRO_HIMHER> to fight longer, harder, and more savagely than any person has a right to.

Advantages:
- +2 bonus to Armor Class.
- +1 to attack and damage rolls every 3 levels.
- -1 bonus to Speed Factor every 4 levels.
- May use the Enrage ability. Gains one use at level 1 and an additional use every 4 levels thereafter.

ENRAGE: For 1 turn, the character gains a +2 bonus to attack and damage rolls, a +2 bonus to Armor Class, and immunity to charm, confusion, fear, feeblemind, hold, imprisonment, level drain, maze, stun, and sleep. The character also gains 15 temporary Hit Points which are taken away at the end of the berserk spree, possibly knocking <PRO_HIMHER> unconscious.

Disadvantages:
- Becomes winded after berserking: -2 penalty to attack rolls, damage, and Armor Class.
- May not wear any armor.
- May not use missile weapons.
- May not wear gauntlets or bracers.
- Alignment restricted to any non-lawful.

---
  
</details>

<details>
  <summary>Monastery Swordsman (monk) - EE only</summary>
  
---

MONASTERY SWORDSMAN: Monks are warriors who pursue perfection through contemplation as well as action. Among them are a subset that have been specially trained to be one with their favored weapons. This Monk's best known feat is the ability to sever an opponent with a single strike.

Advantages:
- May achieve Grand Mastery (five slots) in any weapon available to Monks.
- May place 2 slots in Single Weapon Style and 3 slots in Two-Weapon Style.
- +1 to attack and damage rolls at 3rd level and an additional +1 bonus every 5 levels thereafter.
- Gains ki points, which are used to activate kit abilities. Gains 1 ki point every 3 levels, up to a maximum of 10 points at level 30.
- 3rd level: May use the Element—Fire, Element—Wind, and Element—Moon abilities. Each requires 1 ki point.

ELEMENT—FIRE/WIND/MOON: For 4 rounds, each successful melee attack deals an extra 2d6 fire, slashing, or magic damage. Only one element can be in effect at a time.

- 13th level: May use the Sever ability. Requires 1 ki point.

SEVER: A single deadly strike. The next successful attack within 2 rounds forces the target to make a save vs. Death at -2 or die. An opponent that survives the attack still suffers 5d6 slashing damage.

Disadvantages:
- Unarmed attacks do not gain extra Attacks Per Round bonuses.
- May not use the Stunning Blow ability.
- May not use the Quivering Palm ability.
- May not use slings or darts.

---

</details>

<details>
  <summary>Jesterblade (bard)         - EE and classic</summary>
  
---

JESTERBLADE: The Jesterblade is well versed in the arts of ridicule and hilarity, and uses <PRO_HISHER> abilities to confuse enemies, cavorting madly during combat. Do not mistake <PRO_HIMHER> for a true fool, however. This bard is an expert fighter and adventurer, whose fighting style is lethally dangerous.

Advantages:
- The Jesterblade's song confuses enemies within 30 feet unless they save vs. Spell at a +2 bonus. The bonus lowers to +1 at level 5, +0 at level 10, -1 at level 15, and -2 at level 20.
- May place 3 slots in Two-Weapon Style.
- May use the Offensive Spin and Defensive Spin abilities once per day. Gains one use each at level 1 and an additional use each every 4 levels thereafter.

OFFENSIVE SPIN: During the next 4 rounds, the character gains a +2 bonus to attack and damage rolls, an extra attack per round, doubled movement rate, and all attacks deal maximum damage for the duration. Offensive Spin may not be used in conjunction with the Haste or Improved Haste spells.

DEFENSIVE SPIN: During the next 4 rounds, the character is rooted to the spot and gains a +1 bonus to Armor Class per level, up to a maximum of +10.
  
Disadvantages:
- Bard Song does not gain additional effects at higher levels.
- Only has one half the normal Lore value.
- Only has one half the normal Pick Pockets skill.

---
  
</details>

--

### Components:
1. Install kits
2. Choose Enrage version (options in installer)
3. Update HLAs (only relevant if HLAs were revised)

--

**Notes:**
- config.ini: Set a kit to = 0 to prevent install
- Update HLAs: safe to install after Talents of Faerun. ToF "minor abilities" that require a level check for Blade are not selectable by Jesterblade. One of these, Ambidexterity, will be given to the Jesterblade for free at level 20.


#

#### a few notes on the ki system (Monastery Swordsman):
- Abilities are sometimes removed and re-added (i.e. after resting or loading a save file). This is why sometimes the abilities will be missing temporarily from the menu.
- If abilities are given in the wrong amounts, using any ability should correct the number. The amount given is based on an internal proficiency value that changes each time using an ability (and resets on Rest).
- Any other glitchiness can usually be fixed by opening/closing inventory, or waiting a few extra seconds. Resting will also reset the internal values.
