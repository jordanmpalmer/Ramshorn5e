---
JumpInputStrength: 1.5
---

# Jump Calculator

`INPUT[number:JumpInputStrength]`

Long Jump with running start: `VIEW[{JumpInputStrength}]`
Long Jump from standing: `VIEW[{JumpInputStrength}/2]`
High Jump with running start: `VIEW[(({JumpInputStrength}-10)/2)+3]`
High jump from standing: `VIEW[round((({JumpInputStrength}-10)/2)+3)/2]`
