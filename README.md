
#1.	What is it?

The LiD Calculator is an attempt to have an interactive damage calculator for Let it Die. It is in its very early stages and will be updated frequently as I expand its functionality, learn more about how the game handles attack/damage calculations, and fix my mistakes.

The LiD calculator is a spreadsheet. As such, the intention is to keep it 100% compatible between MS Excel and Google Sheets. This means lots of cell formulas that both platforms handle slightly differently in some cases. Being restricted to what I can do through cell formulas makes things messy. I could get more done and faster using VBA or Google Apps scripts, but that would destroy compatibility between platforms and introduce security concerns for some users of the calculator. I could write the calculator as a web page or web app that could be accessed by basically anyone, anywhere, but I know next to nothing about web development. So, Google Sheets it is.

#2.	Current Status

Currently, the calculator is somewhere between a proof of concept and a functioning tool. It only takes into account how up to 9 decals affect final attack power given a user-supplied ATK value, raw and elemental damage types and percentages, headshot multiplier and base critical damage chance. I have only included decals that affect base attack/damage, critical chance and critical damage. There is currently no functionality to apply different levels of buffs/multipliers for set decals. If you select Trigger Happy or ANGRY MAMA, you’re going to see the full-set multipliers. The calculations also do not take into account STR and DEX scaling, and so consequently do not take into account fighter stats. All calculations are done just on the weapon ATK value, making the results very far from what actually happens in game.

As it is now, it may be useful for being able to see how different weapon and decal combinations perform in a general sense. The calculator currently should not be considered accurate. You may be able to trust that one decal combination is better or worse than another, but you cannot trust that the values shown are what the game itself is working with.

#3.	Features

	●	Ability to specify ATK, damage types and headshot multiplier for a hypothetical weapon. You can reference the LiD Wiki for actual weapon stats.
	●	Ability to specify a base critical hit chance. This is meant to reflect the critical chance from a fighter’s LUK.
	●	Ability to choose up to 9 decals and see their relevant information.
	●	Display of which decal ATK multipliers are actually being applied based on required weapon type, raw and elemental types.
	●	A list of individual decal “group” multipliers for decals that are additive with each other.
	●	A final ATK multiplier (calculated by multiplying each of the group multipliers together)
	●	An explosive round multiplier.
	●	A headshot multiplier.
	●	Final critical chance and critical damage multiplier.
	●	Final ATK values for
		○	Non-critical attacks
	○	Critical attacks
	○	Average attack (based on critical chance)
	○	Non-critical headshot
	○	Critical headshots

#5.	To-Do

A lot. 

A short list of what I’ll most likely implement next is
	
	●	Calculate non-crit and crit rage move damages
	●	Supply a LUK/Crit % table
	●	Supply a fighter stat table
	●	Supply a weapon type (Axe, Katana, Sword, etc…) table and drop-down selection
	●	Implement base stat specification for 3 left-hand and 3 right-hand weapons and the ability to select which weapon is currently being held in each hand

	

