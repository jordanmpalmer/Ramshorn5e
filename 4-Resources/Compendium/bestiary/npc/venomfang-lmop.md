---
obsidianUIMode: preview
cssclasses: json5e-monster
tags:
- compendium/src/5e/lmop
- monster/cr/8
- monster/size/large
- monster/type/dragon
statblock: inline
aliases: ["Venomfang"]
---
```statblock
"name": "Venomfang (LMoP)"
"size": "Large"
"type": "dragon"
"alignment": "Lawful Evil"
"ac": !!int "18"
"hp": !!int "136"
"hit_dice": "16d10 + 48"
"stats":
- !!int "19"
- !!int "12"
- !!int "17"
- !!int "16"
- !!int "13"
- !!int "15"
"speed": "40 ft., fly 80 ft., swim 40 ft."
"saves":
  "Charisma": !!int "5"
  "Dexterity": !!int "4"
  "Wisdom": !!int "4"
  "Constitution": !!int "6"
"skillsaves":
  "Deception": !!int "5"
  "Stealth": !!int "4"
  "Perception": !!int "7"
"damage_immunities": "poison"
"condition_immunities": "[poisoned](4-Resources/Compendium/rules/conditions.md#poisoned)"
"senses": "blindsight 30 ft., darkvision 120 ft., passive Perception 17"
"languages": "Common, Draconic"
"cr": "8"
"traits":
- "desc": "Venomfang can breathe air and water."
  "name": "Amphibious"
"actions":
- "desc": "Venomfang makes three attacks: one with its bite and two with its claws."
  "name": "Multiattack"
- "desc": "Melee Weapon Attack: dice: d20+7 (+7 to hit), reach 10 ft., one target.\
    \ Hit: dice: 2d10 + 4|avg (2d10 + 4) piercing damage plus dice: 2d6|avg\
    \ (2d6) poison damage."
  "name": "Bite"
- "desc": "Melee Weapon Attack: dice: d20+7 (+7 to hit), reach 5 ft., one target.\
    \ Hit: dice: 2d6 + 4|avg (2d6 + 4) slashing damage."
  "name": "Claw"
- "desc": "Venomfang exhales poisonous gas in a 30-foot cone. Each creature in that\
    \ area must make a DC 14 Constitution saving throw, taking dice: 12d6|avg (12d6)\
    \ poison damage on a failed save, or half as much damage on a successful one."
  "name": "Poison Breath (Recharge 5-6)"
"source":
- "LMoP"
"image": "4-Resources/Compendium/bestiary/npc/token/venomfang.png"
```
^statblock
# [Venomfang](4-Resources/Compendium/bestiary/npc/venomfang-lmop.md)
*Source: Lost Mine of Phandelver p. 63, Derived from *