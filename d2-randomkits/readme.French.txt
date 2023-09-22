GitHub: https://github.com/D2-mods/Misc-kits

Notes:
- Compatible avec les Enhanced Editions et sur BG2 original
- Mod made with Notepad++, WeiDU, and Near Infinity
- Utilise ADD_KIT_EX fonction par Argent77 (https://github.com/Argent77/A7-add_kit_ex)
- LibIconv (http://gnuwin32.sourceforge.net/packages/libiconv.htm)


//Kits
Kensaizerker (Kit de guerrier)   - Enhanced Editions et BG2 original
Adepte de l'épée (Kit de moine)  - Enhanced Editions uniquement
Bouffon cinglant (Kit de barde)  - Enhanced Editions et BG2 original

//Fichier "config.ini"
- Mettez la valeur d'un kit à = 0 pour ne pas l'installer


Traductions :
- Français (par 11jo)

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------

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