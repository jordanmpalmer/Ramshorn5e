---
transportation: "walking"
speed: "normal"
exhaustionLevel: 0
hoursPerDay: 8
---

This party is traveling by `=this.transportation`.

This party is traveling by `=[[Transportation]].movement[this.transportation].name`.

It has a base speed of `=[[Transportation]].movement[this.transportation].base` and takes `=[[Transportation]].movement[this.transportation].normal` minutes to go one mile. 

## Calculate Speed

Current speed - `= round(160 * ([[Transportation]].movement[[[Current Party]].transportation][[[Current Party]].speed] * choice([[Current Party]].exhaustionLevel > 1, 2, 1)) / 60 / [[Current Party]].hoursPerDay, 0)` mph

`= [[Transportation]].movement[[[Current Party]].transportation][[[Current Party]].speed]`

Exhaustion level - `= [[Current Party]].exhaustionLevel`

Hours per day - `= [[Current Party]].hoursPerDay`

`= [[Transportation]].movement[[[Current Party]].transportation][[[Current Party]].speed]`