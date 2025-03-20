
GitHub: https://github.com/D2-mods/Misc-kits
Téléchargement : https://github.com/D2-mods/Misc-kits/releases
Langages : English, French

--

Présentation :

- Compatible avec les Enhanced Editions et sur BG2 original
- Quelques kits que j'ai réalisés pour m'entraîner.
- Les tables de capacités sont créés en clonant celles du Kit ou de la Classe de base.


--

v3.0 update :
- L'Adepte de l'épée utilise dorénavant le système d'énergie mystique (aussi utilisé par l'Urgentiste du Workshop Kitpack).
- Ajout du Kit Updater, Utiliser ce composant après tous les mods de tweak et autres overhauls (une possible exception pour le mod Dual to Kit).
- Amélioration de la compatibilité avec les mods de tweak et autres overhauls (Particulièrement avec Talents of Faerun, les mods modifiants les HLAs, et les compétences d'armes).
- BG2 (classique): Ajout d'un variant rôdeur pour l'Adepte de l'épée.


//Kits
Kensaizerker (Kit de guerrier)   - Enhanced Editions et BG2 original
Adepte de l'épée (Kit de moine)  - Enhanced Editions uniquement
Bouffon cinglant (Kit de barde)  - Enhanced Editions et BG2 original
Adepte de l'épée (Kit de rôdeur) - BG2 original uniquement

Composants
1. Installation des kits
2. Choisir la version de la capacité Enragé du Kensaizerker
3. Kit Updater (voir ci-dessous)

--

//Notes d'installation

- Fichier "config.ini" :  
	. Mettez la valeur d'un kit à = 0 pour ne pas l'installer
- Composants Kit Updater et Enragé (Peut être installé en toute sécurité en fin d'installation et réinstallé à tout moment.)


Traductions :
- Français (JohnBob)

Functions (not including my own):
- ADD_KIT_EX function by Argent77 (https://github.com/Argent77/A7-add_kit_ex)
- CD_EXTEND-O-MATIC function by CamDawg (https://www.gibberlings3.net/forums/topic/28835-toss-your-semi-useful-weidu-macros-here/page/13/#comment-332943)
- GET_KIT_STRREF (source unknown)

Older (v2.x) ki system:
- semi_innate_casting function by subtledoctor (https://github.com/subtledoctor/SD_useful_functions)

Outils :
- Notepad++, WeiDU et Near Infinity
- LibIconv (http://gnuwin32.sourceforge.net/packages/libiconv.htm)

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------

v3.1
- ToF note: The kit updater now adds back a line for Monastery Swordsman if overwritten by ToF or another mod (the one that says it starts specialized in single weapon/two-handed weapon).
- Tof note: Monastery Swordsman should no longer be able to put points in bows/crossbows if using the ToF proficiency system. Run the Kit Updater to fix. This edits the line for the kit in m_dw_krd.lua and backs up an unmodified copy in weidu_external/d2mk folder.
- Tof note: Minor fix if using ToF proficiency system (monastery swordsman couldn't put 5 points in staff). Run the Kit Updater to fix. This edits the line for the kit in m_dw_krd.lua and backs up an unmodified copy in weidu_external/d2mk folder.
- BG2 (classic): Minor compat adjustment. (note: if using a monk revision and the AC for Monastery Swordsman looks too low, check the monk class AC to see if the revision is causing it. Even though it's a ranger kit for non-EE, it still uses the monk table as the base before edits.)

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
- Fixed possible install error on Mac systems, caused by using text files without extensions.
- EEs: Monastery Swordsman now starts with 2 slots in Single Weapon Style, matching what a fighter class could do at level 1 (note: for compatibility, single weapon is not removed from the prof screen, so don't put points at creation. A tweak mod can increase the max number of points in weapon styles.)
- Monastery Swordsman: If using a tweak that lets monks use 2-handed weapons, it also starts with 2 points in 2-handed style. You can re-run the updater at any time to recheck this. The description is also updated to match the current files.

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
Kensaizerker (Kit de Guerrier)
==================================================
KENSAIZERKER : Proche du kensai, ou « Seigneur de l'épée », ce guerrier est en phase avec son côté animal et peut atteindre un état d'extase qui lui permet de se battre plus longtemps, plus durement et plus sauvagement, au-delà de toute raison.

Avantages :
– Bonus de 2 à la classe d'armure.
– Bonus de 1 aux jets d'attaque et de dégâts tout les 3 niveaux.
– Bonus de 1 au facteur de vitesse tout les 4 niveaux.
– Peut utiliser la capacité « Enragé » une fois par jour au niveau 1, puis une fois supplémentaire tous les 4 niveaux.

ENRAGÉ : Pendant 1 tour, le personnage gagne un bonus de 2 à sa classe d'armure, à ses jets d'attaque et de dégâts, il bénéficie d'une immunité au charme, à la confusion, à la peur, à la débilité mentale, à l'immobilisation, à l'emprisonnement, au drainage de niveau, au sort de labyrinthe, à l'étourdissement et au sommeil. Le personnage reçoit également 15 points de vie supplémentaires qui seront retirés lorsque sa fureur prendra fin, ce qui peut entraîner une perte de connaissance.

Inconvénients : 
– Suite à sa fureur, le personnage est essoufflé et subit une pénalité de 2 à la classe d'armure, aux jets d'attaque et aux jets de dégâts.
– Ne peut porter aucune armure.
– Ne peut utiliser des armes à distance.
– Ne peut porter de gantelets ou de bracelets.
– Ne peut pas être d'alignement loyal.


==================================================
Monastery Swordsman (Kit de Moine)
==================================================
ADEPTE DE L'ÉPÉE : Les moines sont des guerriers qui cherchent la perfection à travers la contemplation et l'action. Parmi eux, certains ont été spécialement formés pour ne faire qu'un avec leurs armes de prédilection. Le prouesse la plus connue des moines est leur aptitude à couper en deux un adversaire d'un seul coup.

Avantages :
– Bénéficie de la spécialisation à la création (2 points de compétence) dans n'importe quel style de combat à une main.
- Peut allouer trois points de compétence dans le style de combat à deux armes.
– Bonus de 1 aux jets d'attaque et de dégâts au niveau 3, puis une fois supplémentaire tous les 5 niveaux.
– Peut atteindre la grande maîtrise (5 points de compétence) avec les armes de mêlé utilisable par les moines.
– Obtient une quantité d'énergie mystique, qui sera utilisée pour activer les capacités de l'Adepte de l'épée. Bonus de 1 unité d'énergie mystique à chaque montée de niveau, jusqu' au niveau 20.
- Accumulation d'énergie : Cette capacité passive permet de régénérer 1 unité d'énergie mystique tout les 5 rounds.

– 3ème niveau : Peut utiliser la capacité élémentaire « Brasier » (Consomme 3 unités d'énergie mystique).

BRASIER ÉLÉMENTAIRE : Ses attaques de mêlée infligent 2d6 points de dégâts de feu supplémentaires à chaque coup pendant 4 round.

- 5ème niveau : Peut utiliser la capacité élémentaire « Zéphyr » (Consomme 3 unités d'énergie mystique).

ZÉPHYR ÉLÉMENTAIRE : Ses attaques de mêlée infligent 2d6 points de dégâts tranchants supplémentaires à chaque coup pendant 4 round.

- 7ème niveau : Peut utiliser la capacité élémentaire « Lune » (Consomme 3 unités d'énergie mystique).

LUNE ÉLÉMENTAIRE : Ses attaques de mêlée infligent 2d6 points de dégâts magiques supplémentaires à chaque coup pendant 4 round.

- 13ème niveau : Peut utiliser la capacité « Vorpal » (Consomme 6 unités d'énergie mystique).

VORPAL : Un seul coup mais un coup mortel. La prochaine attaque réussie sous 2 rounds tue la cible si celle-ci échoue son jet de sauvegarde contre la mort à -2. Un adversaire qui survit à l'attaque subit tout de même 5d6 points de dégâts tranchants.

Inconvénients :   
- Les attaques à mains nues ne bénéficient pas du bonus d'attaques par round..
- Ne peut utiliser « Coup étourdissant ».
- Ne peut utiliser « Paume tremblante ».
- Ne peut utiliser les frondes et les fléchettes.


==================================================
Jesterblade (Kit de Barde)
==================================================
BOUFFON CINGLANT : Le Bouffon cinglant est versé dans l'art du ridicule et de la plaisanterie, il utilise ses capacités pour déconcerter ses ennemis en cabriolant joyeusement. Cependant, vous feriez mieux de le prendre au sérieux. Ce barde est un expert du combat et un grand aventurier, avec un style... mortel.

Avantages :
– Le chant du barde du Bouffon cinglant n'aide pas ses alliés. Au contraire, elle affecte tous les ennemis dans un rayon de 10 m, qui doivent réussir un jet de sauvegarde contre les sorts à -2 ou devenir confus pendant 1 round.
– Peut allouer trois étoiles dans le style de combat à deux armes.
– Peut utiliser les capacités « spirale offensive » et « spirale défensive » une fois par jour au niveau 1, puis une fois supplémentaire tous les 4 niveaux.

SPIRALE OFFENSIVE : Durant les 4 prochains rounds, la vitesse de déplacement du personnage est doublée et il obtient un bonus de 2 au toucher et aux dégâts, ainsi qu'une attaque supplémentaire par round, et toutes ses attaques font le maximum de dégâts. Ne peut être utilisée en conjonction avec les sorts profanes Hâte ou Hâte améliorée.

SPIRALE DÉFENSIVE : Durant les 4 prochains rounds, le personnage ne peut plus se déplacer, mais obtient un bonus de 1 à sa classe d'armure par niveau d'expérience, jusqu'à un maximum de 10.

Inconvénients : 
– Le chant du barde ne gagne pas d'effet additionnels à haut niveau.
– Score de connaissances divisé par deux.
– Score de Vol à la tire divisé par deux.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------

//alt kit for classic BG2

==================================================
Monastery Swordsman (Ranger)
==================================================
MONASTERY SWORDSMAN: These finely skilled warriors channel a subtle energy, called ki, to perform amazing feats. Their best known feat is the ability to sever an opponent with a single strike.

Advantages:
- Bénéficie de toutes les capacités passives du moine à l’exception de l'amélioration des attaques à mains nues.
– Bonus de 1 aux jets d'attaque et de dégâts au niveau 3, puis une fois supplémentaire tous les 5 niveaux.
– Peut atteindre la grande maîtrise (5 points de compétence) avec les armes de mêlé utilisable par les voleurs.

– 3ème niveau : Peut utiliser la capacité élémentaire « Brasier » une fois par jour, puis une fois supplémentaire au niveau 8 et 20.

BRASIER ÉLÉMENTAIRE : Ses attaques de mêlée infligent 2d6 points de dégâts de feu supplémentaires à chaque coup pendant 4 round.

- 6ème niveau : Peut utiliser la capacité élémentaire « Zéphyr » une fois par jour, puis une fois supplémentaire au niveau 11 et 20.

ZÉPHYR ÉLÉMENTAIRE : Ses attaques de mêlée infligent 2d6 points de dégâts tranchants supplémentaires à chaque coup pendant 4 round.

-  7ème niveau : Peut utiliser  « Imposition des mains » pour soigner 2 points de vie pas niveau.

- 9ème niveau : Peut utiliser la capacité élémentaire « Lune » une fois par jour, puis une fois supplémentaire au niveau 11 et 20.

LUNE ÉLÉMENTAIRE : Ses attaques de mêlée infligent 2d6 points de dégâts magiques supplémentaires à chaque coup pendant 4 round.

- 13ème niveau : Peut utiliser la capacité « Vorpal » une fois par jour, puis une fois supplémentaire au niveau 18.

VORPAL : Un seul coup mais un coup mortel. La prochaine attaque réussie sous 1 rounds tue la cible si celle-ci échoue son jet de sauvegarde contre la mort à -2. Un adversaire qui survit à l'attaque subit tout de même 5d6 points de dégâts tranchants.

Inconvénients :   
- Ne peut utiliser les frondes et les fléchettes et autres armes à distance.
- Ne peut utiliser d'armure ou de casque.
- Ne peut utiliser de gantelets ou bracelets.
- Ne peut utiliser de bouclier.
- Ne peut utiliser « Charme animal ».
- Ne peut accéder aux sorts de prêtre.
- Ne peut être d'alignement chaotique.

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------