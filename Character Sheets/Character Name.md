---
number: 55
number2: 1
toggle3: X
toggle2: X
toggle1: X
n1: 105
n3: 1000
toggle4: X
toggle5: X
n2: 
c: 105
textArea: ""
nG: 0
nS: 5
pp: 15
nW: 5
nD: 4
nC: 2
nI: 2
nCh: 2
togAc: false
nPB: 3
rating: 1
WT: 200
nSS: 10
nDS: 10
nCS: 10
nIS: 10
nWS: 10
nCHS: 10
HD: 4
togAH: false
togIn: false
togPerf: false
togInv: false
togPers: false
togSoH: false
togDe: false
---
# [[Character Name]] - `INPUT[number(class(input-w-least)):n1]`Max/`INPUT[number(class(input-w-least)):n2]`Temp
> [!infobox]
> # Name
> ![[z_Assets/Misc/ImagePlaceholder.png|cover hsmall]]
> [[z_Assets/Misc/ImagePlaceholder.png|Show To Players]]
> ###### Basic Information
Information| Stat |
 ---|---|
 Race |     |
 Level |  `INPUT[inlineSelect(option(1),option(2),option(3),option(4),option(5),option(6),option(7),option(8),option(9),option(10),option(11),option(12),option(13),option(14),option(15),option(16),option(17),option(18),option(19),option(20)):rating]`   |
 Background |     |
 Alignment |     |
 Height/Size |     |
> ###### Backstory
>- This is a place holder **Backstory** that I just wanted to 
# **HP** =`VIEW[{n1} + {n2}][math:c]`
## **Death Saves**: `INPUT[toggle(onValue(✓), offValue(X)):toggle1]` `INPUT[toggle(onValue(✓), offValue(X)):toggle2]` `INPUT[toggle(onValue(✓), offValue(X)):toggle3]` `INPUT[toggle(onValue(✓), offValue(X)):toggle4]` `INPUT[toggle(onValue(✓), offValue(X)):toggle5]`
### **Save Status**: | `VIEW[{toggle1}]` | `VIEW[{toggle2}]` | `VIEW[{toggle3}]` | `VIEW[{toggle4}]` | `VIEW[{toggle5}]` |
### Notes 
`INPUT[textArea(class(input-w-most)):textArea]`

# Stats:

| Armor Class: 10                                  | Initiative: +`VIEW[{nD}]`                                             | Walking Speed: 30ft                                                                                                                                                                                                                                                 |
| :----------------------------------------------- | :-------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Passive Perception: `VIEW[({nW} + 10)][math:pp]` | **Proficiency Bonus**: **+**`INPUT[number(class(input-w-least)):nPB]` | Hit Dice: `INPUT[inlineSelect(option(1),option(2),option(3),option(4),option(5),option(6),option(7),option(8),option(9),option(10),option(11),option(12),option(13),option(14),option(15),option(16),option(17),option(18),option(19),option(20)):HD]`  `dice: 1d8` |

>[!col]
>>[!col-md-1]
>>### Ability Modifiers:
>>| Ability | Modifier |
>>| :---- | :----: |
>>| Strength: | `INPUT[number(class(input-w-some)):nS]` (`INPUT[number(class(input-w-some)):nSS]`) |
>>| Dexterity: | `INPUT[number(class(input-w-some)):nD]` (`INPUT[number(class(input-w-some)):nDS]`) |
>>| Constitution: | `INPUT[number(class(input-w-some)):nC]` (`INPUT[number(class(input-w-some)):nCS]`) |
>>| Intelligence: | `INPUT[number(class(input-w-some)):nI]` (`INPUT[number(class(input-w-some)):nIS]`) |
>>| Wisdom: | `INPUT[number(class(input-w-some)):nW]` (`INPUT[number(class(input-w-some)):nWS]`) |
>>| Charisma: | `INPUT[number(class(input-w-some)):nCh]` (`INPUT[number(class(input-w-some)):nCHS]`) |
>
>>[!col-md-1]
>>### Saving Throw
>>| Ability | Roll |
>>| :---- | :----: |
>>| Strength: | `dice: 1d20` + `VIEW[{nS}]` |
>>| Dexterity: | `dice: 1d20` + `VIEW[{nD}]` |
>>| Constitution: | `dice: 1d20` + `VIEW[{nC}]` |
>>| Intelligence: | `dice: 1d20` + `VIEW[{nI}]` |
>>| Wisdom: | `dice: 1d20` + `VIEW[{nW}]` |
>>| Charisma: | `dice: 1d20` + `VIEW[{nCh}]` |
>
>>[!col-md-4]
>>### Skills:
>>| Skill| Roll |
>>| :---: | :---: |
>>| **Acrobatics** `INPUT[toggle:togAc]` | `dice: 1d20` + `VIEW[{nD}]` + `VIEW[{togAc} ? {nPB}: 0]` |
>>| **Animal Handling** `INPUT[toggle:togAH]` | `dice: 1d20` + `VIEW[{nW}]` + `VIEW[{togAH} ? {nPB}: 0]` |
>>| **Athletics** `INPUT[toggle:togAt]` | `dice: 1d20` + `VIEW[{nS}]` + `VIEW[{togAt} ? {nPB}: 0]` |
>>| **Arcana** `INPUT[toggle:togAr]` | `dice: 1d20` + `VIEW[{nI}]` + `VIEW[{togAr} ? {nPB}: 0]` |
>>| **Deception** `INPUT[toggle:togDe]` | `dice: 1d20` + `VIEW[{nCh}]` + `VIEW[{togDe} ? {nPB}: 0]` |
>>| **History** `INPUT[toggle:togHi]` | `dice: 1d20` + `VIEW[{nI}]` + `VIEW[{togHi} ? {nPB}: 0]` |
>>| **Insight**  `INPUT[toggle:togIn]`| `dice: 1d20` + `VIEW[{nW}]` + `VIEW[{togIn} ? {nPB}: 0]` |
>>| **Intimidation** `INPUT[toggle:togInt]` | `dice: 1d20` + `VIEW[{nCh}]` + `VIEW[{togInt} ? {nPB}: 0]` |
>>| **Investigation** `INPUT[toggle:togInv]` | `dice: 1d20` + `VIEW[{nI}]` + `VIEW[{togInv} ? {nPB}: 0]` |
>>| **Medicine** `INPUT[toggle:togMe]` | `dice: 1d20` + `VIEW[{nW}]` + `VIEW[{togMe} ? {nPB}: 0]` |
>>| **Nature** `INPUT[toggle:togNa]` | `dice: 1d20` + `VIEW[{nI}]` + `VIEW[{togNa} ? {nPB}: 0]` |
>>| **Perception** `INPUT[toggle:togPerc]` | `dice: 1d20` + `VIEW[{nW}]` + `VIEW[{togPerc} ? {nPB}: 0]` |
>>| **Performance** `INPUT[toggle:togPerf]` | `dice: 1d20` + `VIEW[{nCh}]` + `VIEW[{togPerf} ? {nPB}: 0]` |
>>| **Persuasion** `INPUT[toggle:togPers]` | `dice: 1d20` + `VIEW[{nCh}]` + `VIEW[{togPers} ? {nPB}: 0]` |
>>| **Religion** `INPUT[toggle:togRe]` | `dice: 1d20` + `VIEW[{nI}]` + `VIEW[{togRe} ? {nPB}: 0]` |
>>| **Sleight of Hand** `INPUT[toggle:togSoH]` | `dice: 1d20` + `VIEW[{nD}]` + `VIEW[{togSoH} ? {nPB}: 0]` |
>>| **Stealth** `INPUT[toggle:togSt]` | `dice: 1d20` + `VIEW[{nD}]` + `VIEW[{togSt} ? {nPB}: 0]` |
>>| **Survival** `INPUT[toggle:togSu]` | `dice: 1d20` + `VIEW[{nW}]` + `VIEW[{togSu} ? {nPB}: 0]` |
## Feat:
| Feat Name | Ability |
| :-------: | :-----: |
|           |         |

## Pack:
>[!col]
>>[!col-md-1]
>>| Currency |
>>| :--: |
>>| `INPUT[number(class(input-a-right)):nG]`G |
>>| `INPUT[number(class(input-a-right)):nS]`S |
>>| `INPUT[number(class(input-a-right)):nC]`C |
>
>>[!col-md-4]
>>| Equipment | Item Description | Item size | Item Weight |
>>| :-------: | ---------------- | --------- | ----------- |
>>|           |                  |           |             |
>>**Weight Total: 123/`VIEW[(({nSS} * 10)+100)][math:WT]`**
>>
>>>[!col-md-4]
>>>| Weapon Name | Attack Bonus | Damage |   Damage Type   | Range |
>>>| :-----------------: | :----------: | :----: | :-------------: | :-------: |
>>>| **Unarmed Strike**  | `dice: 1d20`+`VIEW[{nS}]` | `dice: 1d8`+`VIEW[{nS}]` | **Bludgeoning** |  **5ft**  |
>>>|                     |              |        |                 |           |

