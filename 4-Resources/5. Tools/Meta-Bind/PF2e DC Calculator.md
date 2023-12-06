---
InputDCLevel: 19
---

# DC Calculator

**Enter Player Level:** `INPUT[inlineSelect(option(14,Lvl 0 - DC: 14),option(15,Lvl 1 - DC: 15),option(16,Lvl 2 - DC: 16),option(18,Lvl 3 - DC: 18),option(19,Lvl 4 - DC: 19),option(20,Lvl 5 - DC: 20),option(22,Lvl 6 - DC: 22),option(23,Lvl 7 - DC: 23),option(24,Lvl 8 - DC: 24),option(26,Lvl 9 - DC: 26),option(27,Lvl 10 - DC: 27),option(28,Lvl 11 - DC: 28),option(30,Lvl 12 - DC: 30),option(31,Lvl 13 - DC: 31),option(32,Lvl 14 - DC: 32),option(34,Lvl 15 - DC: 34),option(35,Lvl 16 - DC: 35),option(36,Lvl 17 - DC: 36),option(38,Lvl 18 - DC: 38),option(39,Lvl 19 - DC: 39),option(40,Lvl 20 - DC: 40),option(42,Lvl 21 - DC: 42),option(44,Lvl 22 - DC: 44),option(46,Lvl 23 - DC: 46),option(48,Lvl 24 - DC: 48),option(50,Lvl 25 - DC: 50)):InputDCLevel]`

| Challenge Level | DC                        |
| --------------- | ------------------------- |
| Incredibly Easy | `VIEW[{InputDCLevel}-10]` |
| Very Easy       | `VIEW[{InputDCLevel}-5]`  |
| Easy            | `VIEW[{InputDCLevel}-2]`  | 
| Normal          | `VIEW[{InputDCLevel}]`    |
| Hard            | `VIEW[{InputDCLevel}+2]`  |
| Very Hard       | `VIEW[{InputDCLevel}+5]`  |
| Incredibly Hard | `VIEW[{InputDCLevel}+10]` |
