---
number: 55
number2: 1
toggle3: X
toggle2: false
toggle1: true
n1: 0
n3: 1000
toggle4: X
toggle5: X
n2: 0
c: 0
textArea: ""
nG: 0
nS: 0
pp: 10
nW: 0
nD: 0
nC: 0
nI: 0
nCh: 0
togAc: false
nPB: 2
rating: 1
WT: 200
nSS: 10
nDS: 10
nCS: 10
nIS: 10
nWS: 10
nCHS: 10
HD: 1
togAH: false
togIn: false
togPerf: false
togInv: false
togPers: false
togSoH: false
togDe: false
togAcE: false
togAHE: false
togAt: false
togAr: false
togAtE: false
togArE: false
togDeE: false
togHiE: false
togInE: false
togIntE: false
togInvE: false
togMeE: false
togNaE: false
togPercE: false
togPerfE: false
togPersE: false
togReE: false
togSoHE: false
togStE: false
togSuE: false
ProAc: 0
ExpAc: 0
ProAH: 0
ExpAH: 0
ProAt: 0
ExpAt: 0
ProAr: 0
ExpAr: 0
ProDe: 0
De: 0
ExpDe: 0
Exphi: 0
ProHi: 0
togHi: false
ExpIn: 0
ProIn: 0
ExpInt: 0
ProInt: 0
ExpInv: 0
ProInv: 0
ExpMe: 0
ProMe: 0
ExpNa: 0
ProNa: 0
togNa: false
ExpPerc: 0
ProPerc: 0
ProPerf: 0
ExpPerf: 0
ExpPers: 0
ProPers: 0
ExpRe: 0
ProRe: 0
ExpSoH: 0
ProSoH: 0
ExpSt: 0
ProSt: 0
ExpSu: 0
ProSu: 0
togPerc: false
togSu: false
togSt: false
togRe: false
togMe: false
togInt: false
CalcPerc: 0
nChS: 10
lvl: 1
TPB: 3
ProStre: 0
togStre: false
togDext: false
togCons: false
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
 Level |  `INPUT[inlineSelect(option(1),option(2),option(3),option(4),option(5),option(6),option(7),option(8),option(9),option(10),option(11),option(12),option(13),option(14),option(15),option(16),option(17),option(18),option(19),option(20)):lvl]`   |
 Background |     |
 Alignment |     |
 Height/Size |     |
> ###### Backstory
>- This is a place holder **Backstory** that I just wanted to 
# **HP** =`VIEW[{n1} + {n2}][math:c]`
## **Death Saves**: `INPUT[toggle:toggle1]` `INPUT[toggle:toggle2]` `INPUT[toggle(onValue(✓), offValue(X)):toggle3]` `INPUT[toggle(onValue(✓), offValue(X)):toggle4]` `INPUT[toggle:toggle5]`
### **Save Status**: | `VIEW[{toggle1}]` | `VIEW[{toggle2}]` | `VIEW[{toggle3}]` | `VIEW[{toggle4}]` | `VIEW[{toggle5}]` |
### Notes 
`INPUT[textArea(class(input-wl-most)):textArea]`

# Stats:


| Armor Class: 10                                        | Initiative: +`VIEW[{nD}]`                                   | Walking Speed: 30ft                                                                                                                                                                                                                                                 |
| :----------------------------------------------------- | :---------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Passive Perception: `VIEW[({CalcPerc} + 10)][math:pp]` | **Proficiency Bonus**: **+**`VIEW[ceil({lvl} / 4)+1][:nPB]` | Hit Dice: `INPUT[inlineSelect(option(1),option(2),option(3),option(4),option(5),option(6),option(7),option(8),option(9),option(10),option(11),option(12),option(13),option(14),option(15),option(16),option(17),option(18),option(19),option(20)):HD]`  `dice: 1d8` |

>[!col]
>>[!col-md-1]
>>### Ability Modifiers:
>>| Ability | Modifier |
>>| :---- | :----: |
>>| Strength: | **+**`VIEW[floor(({nSS} - 10)/2)][:nS]` (`INPUT[number(class(input-w-some)):nSS]`) |
>>| Dexterity: | **+**`VIEW[floor(({nDS} - 10)/2)][:nD]` (`INPUT[number(class(input-w-some)):nDS]`) |
>>| Constitution: | **+**`VIEW[floor(({nCS} - 10)/2)][:nC]` (`INPUT[number(class(input-w-some)):nCS]`) |
>>| Intelligence: | **+**`VIEW[floor(({nIS} - 10)/2)][:nI]` (`INPUT[number(class(input-w-some)):nIS]`) |
>>| Wisdom: | **+**`VIEW[floor(({nWS} - 10)/2)][:nW]` (`INPUT[number(class(input-w-some)):nWS]`) |
>>| Charisma: | **+**`VIEW[floor(({nChS} - 10)/2)][:nCh]` (`INPUT[number(class(input-w-some)):nChS]`) |
>
>>[!col-md-1]
>>### Saving Throw
>>| Ability | Roll |
>>| :---- | ----: |
>>| Strength: | `dice: 1d20` `INPUT[toggle:togStre]` + `VIEW[({togStre} ? {nPB}: 0) + {nS}]` |
>>| Dexterity: | `dice: 1d20` `INPUT[toggle:togDext]` + `VIEW[({togDext} ? {nPB}: 0) + {nD}]` |
>>| Constitution: | `dice: 1d20` `INPUT[toggle:togCons]` + `VIEW[({togCons} ? {nPB}: 0) + {nC}]` |
>>| Intelligence: | `dice: 1d20` `INPUT[toggle:togInte]` + `VIEW[({togInte} ? {nPB}: 0) + {nI}]` |
>>| Wisdom: | `dice: 1d20` `INPUT[toggle:togWisd]` + `VIEW[({togWisd} ? {nPB}: 0) + {nW}]` |
>>| Charisma: | `dice: 1d20` `INPUT[toggle:togChar]` + `VIEW[({togChar} ? {nPB}: 0) + {nCh}]` |
>
>>[!col-md-4]
>>### Skills:
>>| Skill | Proficiency | Expertise | Roll |
>>| :--- | :---: | :---: | ---: |
>>| **Acrobatics** | `INPUT[toggle:togAc]` + `VIEW[{togAc} ? {nPB}: 0][:ProAc]` | `INPUT[toggle:togAcE]` + `VIEW[{togAcE} ? {nPB}: 0][:ExpAc]` | `dice: 1d20` + `VIEW[({ProAc} + {ExpAc} + {nD})]` |
>>| **Animal Handling** | `INPUT[toggle:togAH]` + `VIEW[{togAH} ? {nPB}: 0][:ProAH]` | `INPUT[toggle:togAHE]` + `VIEW[{togAHE} ? {nPB}: 0][:ExpAH]` | `dice: 1d20` + `VIEW[({ProAH} + {ExpAH} + {nW})]` |
>>| **Athletics** | `INPUT[toggle:togAt]` + `VIEW[{togAt} ? {nPB}: 0][:ProAt]` | `INPUT[toggle:togAtE]` + `VIEW[{togAtE} ? {nPB}: 0][:ExpAt]` | `dice: 1d20` + `VIEW[({ProAt} + {ExpAt} + {nS})]` |
>>| **Arcana** | `INPUT[toggle:togAr]` + `VIEW[{togAr} ? {nPB}: 0][:ProAr]` | `INPUT[toggle:togArE]` + `VIEW[{togArE} ? {nPB}: 0][:ExpAr]` | `dice: 1d20` + `VIEW[({ProAr} + {ExpAr} + {nI})]` |
>>| **Deception** | `INPUT[toggle:togDe]` + `VIEW[{togDe} ? {nPB}: 0][:ProDe]` | `INPUT[toggle:togDeE]` + `VIEW[{togDeE} ? {nPB}: 0][:ExpDe]` | `dice: 1d20` + `VIEW[({ProDe} + {ExpDe} + {nCh})]` |
>>| **History** | `INPUT[toggle:togHi]` + `VIEW[{togHi} ? {nPB}: 0][:ProHi]` | `INPUT[toggle:togHiE]` + `VIEW[{togHiE} ? {nPB}: 0][:Exphi]` | `dice: 1d20` + `VIEW[({ProHi} + {ExpHi} + {nI})]` |
>>| **Insight** | `INPUT[toggle:togIn]` + `VIEW[{togIn} ? {nPB}: 0][:ProIn]` | `INPUT[toggle:togInE]` + `VIEW[{togInE} ? {nPB}: 0][:ExpIn]` | `dice: 1d20` + `VIEW[({ProIn} + {ExpIn} + {nW})]` |
>>| **Intimidation** | `INPUT[toggle:togInt]` + `VIEW[{togInt} ? {nPB}: 0][:ProInt]` | `INPUT[toggle:togIntE]` + `VIEW[{togIntE} ? {nPB}: 0][:ExpInt]` | `dice: 1d20` + `VIEW[({ProInt} + {ExpInt} + {nCh})]` |
>>| **Investigation** | `INPUT[toggle:togInv]` + `VIEW[{togInv} ? {nPB}: 0][:ProInv]` | `INPUT[toggle:togInvE]` + `VIEW[{togInvE} ? {nPB}: 0][:ExpInv]` | `dice: 1d20` + `VIEW[({ProInv} + {ExpInv} + {nI})]` |
>>| **Medicine** | `INPUT[toggle:togMe]` + `VIEW[{togMe} ? {nPB}: 0][:ProMe]` | `INPUT[toggle:togMeE]` + `VIEW[{togMeE} ? {nPB}: 0][:ExpMe]` | `dice: 1d20` + `VIEW[({ProMe} + {ExpMe} + {nW})]` |
>>| **Nature** | `INPUT[toggle:togNa]` + `VIEW[{togNa} ? {nPB}: 0][:ProNa]` | `INPUT[toggle:togNaE]` + `VIEW[{togNaE} ? {nPB}: 0][:ExpNa]` | `dice: 1d20` + `VIEW[({ProNa} + {ExpNa} + {nI})]` |
>>| **Perception** | `INPUT[toggle:togPerc]` + `VIEW[{togPerc} ? {nPB}: 0][:ProPerc]` | `INPUT[toggle:togPercE]` + `VIEW[{togPercE} ? {nPB}: 0][:ExpPerc]` | `dice: 1d20` + `VIEW[({ProPerc} + {ExpPerc} + {nW})][:CalcPerc]` |
>>| **Performance** | `INPUT[toggle:togPerf]` + `VIEW[{togPerf} ? {nPB}: 0][:ProPerf]` | `INPUT[toggle:togPerfE]` + `VIEW[{togPerfE} ? {nPB}: 0][:ExpPerf]` | `dice: 1d20` + `VIEW[({ProPerf} + {ExpPerf} + {nCh})]` |
>>| **Persuasion** | `INPUT[toggle:togPers]` + `VIEW[{togPers} ? {nPB}: 0][:ProPers]` | `INPUT[toggle:togPersE]` + `VIEW[{togPersE} ? {nPB}: 0][:ExpPers]` | `dice: 1d20` + `VIEW[({ProPers} + {ExpPers} + {nCh})]`|
>>| **Religion** | `INPUT[toggle:togRe]` + `VIEW[{togRe} ? {nPB}: 0][:ProRe]` | `INPUT[toggle:togReE]` + `VIEW[{togReE} ? {nPB}: 0][:ExpRe]` | `dice: 1d20` + `VIEW[({ProRe} + {ExpRe} + {nI})]` |
>>| **Sleight of Hand** | `INPUT[toggle:togSoH]` + `VIEW[{togSoH} ? {nPB}: 0][:ProSoH]` | `INPUT[toggle:togSoHE]` + `VIEW[{togSoHE} ? {nPB}: 0][:ExpSoH]` | `dice: 1d20` + `VIEW[({ProSoH} + {ExpSoH} + {nD})]` |
>>| **Stealth** | `INPUT[toggle:togSt]` + `VIEW[{togSt} ? {nPB}: 0][:ProSt]` | `INPUT[toggle:togStE]` + `VIEW[{togStE} ? {nPB}: 0][:ExpSt]` | `dice: 1d20` + `VIEW[({ProSt} + {ExpSt} + {nD})]` |
>>| **Survival** | `INPUT[toggle:togSu]` + `VIEW[{togSu} ? {nPB}: 0][:ProSu]` | `INPUT[toggle:togSuE]` + `VIEW[{togSuE} ? {nPB}: 0][:ExpSu]` | `dice: 1d20` + `VIEW[({ProSu} + {ExpSu} + {nW})]` |
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
>>| `INPUT[number(class(input-a-right)):nSi]`S |
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

