GitHub: https://github.com/D2-mods/Misc-kits

Notes:
- Compatible avec les Enhanced Editions et BG2 original
- Utilise ADD_KIT_EX fonction par Argent77 (https://github.com/Argent77/A7-add_kit_ex)
- Utilise semi_innate_casting fonction par subtledoctor (https://github.com/subtledoctor/SD_useful_functions)
- Utilise CD_EXTEND-O-MATIC fonction par CamDawg (https://www.gibberlings3.net/forums/topic/28835-toss-your-semi-useful-weidu-macros-here/page/13/#comment-332943)


//Kits
Kensaizerker (Kit de guerrier)   - Enhanced Editions et BG2 original
Adepte de l'épée (Kit de moine)  - Enhanced Editions uniquement
Bouffon cinglant (Kit de barde)  - Enhanced Editions et BG2 original

Composants
1. Installation des kits
2. Choisir la version de la capacité Enragé du Kensaizerker
3. Mettre à jour les HLA (ce composant n'est utile que si les capacités de haut niveau ont été modifiées après l'installation de ce mod)

--

//Notes

- Fichier "config.ini" :  
	. Mettez la valeur d'un kit à = 0 pour ne pas l'installer
- Composant Mettre à jour les HLAs :  
	. Ce composant peut être installé sans problème après Talents of Faerun. (Les « capacités mineures » de ToF qui nécessitent de déterminer le niveau du Bouffon cinglant ne peuvent pas être sélectionnées par celui-ci. L'une d'entre elles, l'Ambidextérité, sera attribuée au Bouffon cinglant au niveau 20.)


Traductions :
- Français (par 11jo)

Outils :
- Notepad++, WeiDU et Near Infinity
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
– Peut atteindre la grande maîtrise (4 points de compétence) avec les armes utilisable par les moines.
– Peut se spécialiser (2 points de compétence) dans n'importe quel style de combat à une main, et allouer trois étoiles dans le style de combat à deux armes.
– Bonus de 1 aux jets d'attaque et de dégâts tout les 4 niveaux.
– 2ème niveau : Peut utiliser la capacité « Brasier » une fois par jour, puis une fois supplémentaire tous les 4 niveaux.

BRASIER : Le moine canalise sa lumière intérieure, enveloppant ses armes d'une flamme vive, mais éphémère. Les attaques de mêlée infligent 2d6 points de dégâts de feu supplémentaires à chaque coup pendant 1 round. Cette durée passe à 2 rounds au niveau 9, à 3 rounds au niveau 12, à 4 rounds au niveau 15, et à 5 rounds au niveau 25.

– 13ème niveau : Peut utiliser la capacité « Vorpal » une fois par jour.

VORPAL : Un seul coup mais un coup mortel. La prochaine attaque réussie sous 2 rounds tue la cible si celle-ci échoue son jet de sauvegarde contre la mort à -2. Un adversaire qui survit à l'attaque subit tout de même 5d6 points de dégâts tranchants.

Inconvénients : 
– Les attaques à mains nues ne bénéficient pas du bonus d'attaques par round..
– Ne peut utiliser « Coup étourdissant ».
– Ne peut utiliser « Paume tremblante ».
– Ne peut utiliser les frondes et les fléchettes.


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