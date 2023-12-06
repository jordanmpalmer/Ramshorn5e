---
publish: true
time: 09:12
date2: 2024-10-17
date1: 2024-07-07
editor1: |-
  # Heading
  test
  test

  more test

  ### Heading 3
image: z_Assets/NPC_Placeholder.png
select: 1
select2: 1
select3: 2 hours
list:
  - Option 1
  - Another option
slider1: 87
slider2: 6
slider3: 526
fileSuggest2: "[[2-Mechanics/Compendium/spells/blindness-deafness.md|blindness-deafness]]"
fileSuggest: "[[2-Mechanics/Compendium/spells/spider-climb.md|spider-climb]]"
toggle1: false
toggle2: 0
text: this is text
textArea: |-
  Test
  More text

  This is more text
suggest: option 3
multiSelect:
  - option 1
  - option 2
  - option 3
JumpInputStrength: 45
number: 55
toggle3: off
text2: this is new
text3: asdasd
number2: 100
progress1: -7
---

# Meta Bind Examples

#### Plugin Link
[Meta Bind](obsidian://show-plugin?id=obsidian-meta-bind-plugin)

### Input Fields
Input fields allow you to create input fields for your notes metadata and interact with them in live preview and reading mode. A bit like properties, but not just at the top of your note.

There are two ways to format the `Input Fields`. 

**Inline:**
`INPUT[text(showcase, title('this is a cool title')):text3]`

**Block:** 
```meta-bind
INPUT[text(showcase, title('this is a cool title')):text3]
```

## Input Examples
### Date
`INPUT[date:date1]` 
`VIEW[{date1}]`

### Date Picker
`INPUT[datePicker:date2]`
`VIEW[{date2}]`

### Time
`INPUT[time:time]`
`VIEW[{time}]`

### Editor
`INPUT[editor:editor1]`
`VIEW[{editor1}]`

### Image Suggestor
`INPUT[imageSuggester(optionQuery("z_Assets")):image]`
`VIEW[{image}]`

### Inline Select

`INPUT[inlineSelect(option(a), option(b)):select]`
`VIEW[{select}]`

`INPUT[inlineSelect(option(1, a), option(2, b)):select2]`
`VIEW[{select2}]`

`INPUT[inlineSelect(option(1 hour, a), option(2 hours, b)):select3]`
`VIEW[{select3}]`
### List

`INPUT[list:list]`
`VIEW[{list}]`

### Number

`INPUT[number:number]`
`VIEW[{number}]`

### Default Value
`INPUT[number(defaultValue(100)):number2]`
`VIEW[{number2}]`



### Progress Bar

`INPUT[progressBar(minValue(-10), maxValue(3)):progress1]`
`VIEW[{progress1}]`
### Select

`INPUT[select(option(1, option 1), option(2, option 2), option(3, option 3)):select]`
`VIEW[{select}]`

`INPUT[select(option(1, option 1), option(false, option 2), option(null, option 3)):select2]`
`VIEW[{select2}]`
### Multi Select

`INPUT[multiSelect(option(option 1), option(option 2), option(option 3)):multiSelect]`
`VIEW[{multiSelect}]`
### Simple Slider

`INPUT[slider:slider1]`
`VIEW[{slider1}]`
### Slider with Labels

`INPUT[slider(addLabels):slider1]`
`VIEW[{slider1}]`
### Slider with custom min max values

`INPUT[slider(addLabels, minValue(-20), maxValue(20)):slider2]`
`VIEW[{slider2}]`

`INPUT[slider(addLabels, minValue(0), maxValue(1000)):slider3]`
`VIEW[{slider3}]`

### Simple Suggester

`INPUT[suggester(option(option 1),option(option 2),option(option 3)):suggest]`
`VIEW[{suggest}]`

### Suggester with Dataview
Note, that this will error, if dataview is not enabled.

`INPUT[suggester(optionQuery(#spell/level/2)):fileSuggest]`
`VIEW[{fileSuggest}]`

### Text
`INPUT[text:text]`
`VIEW[{text}]`

`INPUT[text(placeholder(Appointment Location)):text2]`
`VIEW[{text2}]`

```meta-bind
INPUT[text(showcase, title('this is a cool title')):text3]
```

`VIEW[{text3}]`

### Text Area

`INPUT[textArea(class(meta-bind-full-width), class(meta-bind-high)):textArea]`
`VIEW[{textArea}]`
### Toggle

`INPUT[toggle:toggle1]`
`VIEW[{toggle1}]`

`INPUT[toggle(onValue(1), offValue(0)):toggle2]`
`VIEW[{toggle2}]`

`INPUT[toggle(onValue(on), offValue(off)):toggle3]`
`VIEW[{toggle3}]`

# View Example

View Fields are a powerful way to reactively display your metadata in your notes. They can bind to multiple frontmatter fields and update as soon as you change them, much like dataview inline queries, but with Obsidian Publish support. View Fields use [mathjs expressions](https://mathjs.org/docs/expressions/syntax.html) under the hood.

Calculate multiple properties:
number: `VIEW[{number}]`

`VIEW[{JumpInputStrength}+{number}]`

`INPUT[number:JumpInputStrength]`

Long Jump with running start: `VIEW[{JumpInputStrength}]`
Long Jump from standing: `VIEW[{JumpInputStrength}/2]`
High Jump with running start: `VIEW[(({JumpInputStrength}-10)/2)+3]`
High jump from standing: `VIEW[round((({JumpInputStrength}-10)/2)+3)/2]`

## Reference Properties From Other Notes
Note, that this will error, if you do not have the Party Configuration note in your vault.


`VIEW[{Party Configuration#BaseSpeed}]`

`VIEW[{Party Configuration#DangerLevel}]`

`VIEW[{Party Configuration#BaseSpeed}+{Party Configuration#DangerLevel}]`

