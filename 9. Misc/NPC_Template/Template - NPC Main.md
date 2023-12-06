---
type: NPC
tags: 
associatedFaction: N/A
associatedSubFaction: N/A
TrueAssociatedGroup: N/A
CurrentHome: N/A
ParentLocation: "[[2. Aeonia/Aster/Countries & Regions/Shadowkeep of Aster/Shadowkeep of Aster.md|Shadowkeep of Aster]]"
ExactLocation: "[[2. Aeonia/Kielo/Kielo.md|Kielo]]"
Alignment: True Neutral
heritage:
  - Mr Test
  - Mrs Test
homeland:
  - (Outer Location via MetaBind)
  - (Inner Location via Metabind)
Condition: Unfinished NPC
Age: N/A
Sex: N/A
Race: Race
Height: 
TitleJob: N/A
Class: Class/Role
religion:
  - N/A
skills:
  - N/A
  - N/A
  - N/A
Character-Role: N/A
Strength: N/A
Storylines: N/A
PartyRelation: Unknown
friends:
  - N/A
enemies:
  - N/A
specialtraits: 
---

#NPC 
> [!infobox|right]
> # `=this.file.name`
> ![[NPC_Placeholder.png|cover hsmall]]
> [[NPC_Placeholder.png|Show To Players]]
> ### CR `=this.Strength`
> ###### Basic Information
> Type |  Stat |
> ---|---|
> Home | **`=this.CurrentHome`** |
> Group/Faction | **`=this.associatedFaction`**|
> Occupation | **`=this.TitleJob`** |
> Condition | **`INPUT[TempCondition][:Condition]`** |
> Current Location |**`INPUT[suggester(optionQuery(#region), showcase):ParentLocation]`** |
> Exact Location |**`INPUT[suggester(optionQuery(#continent), showcase):ExactLocation]`** |
> Strength |  **CR `=this.strength`** |
> Relation To Party | `INPUT[TempRelation][:PartyRelation]` |
> ###### Rules Info
> Type |  Stat |
> ---|---|
> Alignment | **`INPUT[TempAlign][:Alignment]`** |
> Class | **`=this.class`** |
> Character Role | **`=this.character-role`** |
> ###### Story Info
> Type |  Stat |
> ---|---|
> True Allegiance | **`=this.TrueAssociatedGroup`** |
> Quests/Story Hooks | **`=this.Storylines`** |
> ###### World Relationship
> Groups/Entities |  Relationship |
> ---|---|
> Friends | **`=this.Friends`** |
> Enemies | **`=this.Enemies`** |


# `=this.file.name`
### `=this.race` • `=this.class` • (Strength Estimation)
##### <center>                    “Character defining personality quote-”               </center>

>[!column| alt-line no-i no-t] 
>>[!info| clean]+ Overview
>> 
>> <br> **Lorem Ipsum** is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum. 
>>   
> 
>> [!info|clean no-icon]  **Appearance**
>> <br> <font color=darkred>**Description:**</font> is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. 
>>  <font color=darkred>**Notable Features:**                                                   </font> 
>> <font color="darkred">**Eyes:**                                                                      </font> 
>> <font color="darkred">**Hair:**                                                                      </font>
>> <font color="darkred">**Height:**                                                                  </font>
>> <font color="darkred">**Build:**                                                                     </font> 

>[!column|flex 3 clean no-title]
>> [!kith|bg-c-gray ]+ <font size=2, color="#595959">**Bio** <sup>_Details of Character_</sup> </font>
>> - **Age:**                       `=this.age`
>> - **Sex:**                        `=this.Sex`
>> - **Race:**                       `=this.race`
>> - **Homeland:** `INPUT[suggester(optionQuery(#region), showcase):ParentLocation]` in `INPUT[suggester(optionQuery(#continent), showcase):ExactLocation]`
>> - **Heritage:**                `=link(this.heritage)`
>
>> [!kith|bg-c-gray]+ <font size=2, color="#595959">**Other Info**<sup> _Life Paths_</sup></font>
>> 
>> - **Current Home:** `=this.Home`
>> - **Group/Guild(s):** `=this.associatedFaction`
>> - **Job/Titles(s):** `=this.GroupTitleJob` 
>> - **Faith(s):** `=this.Religions`
>> - **Skills:** `=this.skills`

>[!column|clean no-title] 
>> [!metadata|bg-c-blue clean]+ Traits & Personality
>> - `=this.traits`
>
>> [!metadata|bg-c-blue clean]+ Ideals, Bonds, & Flaws
>> -  `=this.ideals`
>> -  `=this.bonds`
>> -  `=this.flaws`

>[!column|clean no-icon alt-line]+ DM Notes 
>>[!note|bg-c-blue no-icon clean dim]+ Relationships 
>> <center><sup>Friends, Family, Acquaintances, Neutrals</sup></center>
>> 
>> - [ ] 
>> - [ ] 
>> - [ ] 
>> - [ ] 
>
>>[!note|bg-c-red no-icon clean dim]+ Vendettas  
>> <center><sup>Enemies, Grudges, Rivals, BBEG’s</sup></center>
>> 
>> - [ ] 
>> - [ ] 
>> - [ ] 
>> - [ ] 
>
>>[!note|bg-c-green no-icon clean dim]- Quests/Story Hooks 
>> - [ ] 
>> - [ ] 
>> - [ ] 
>> - [ ] 
>
>>[!info|bg-c-orange clean dim]- Secrets 
>> - [ ] 
>> - [ ] 
>> - [ ] 
>> - [ ] 
>
<center><sub><sub> Checkmark - PC Party is Knowledgeable of that Detail/Hook/Relationship </sub></sub></center>


 



---







>[!info|bg-c-gray clean dim]- ##### DM Scratch Notes
Notes for the DM to  just scratch onto things about plans, designs, intent, story hooks, or quick TODO’s 
































