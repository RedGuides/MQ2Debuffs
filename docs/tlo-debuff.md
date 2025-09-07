---
tags:
  - tlo
---
# `Debuff`

<!--tlo-desc-start-->
Holds the Debuff data type and several forms for pets and specific debuffs
<!--tlo-desc-end-->

## Forms
<!--tlo-forms-start-->
### {{ renderMember(type='bool', name='Debuff') }}

:   True if you have debuffs on that have counters on them, false if not

### {{ renderMember(type='Debuff', name='Debuff', params='self') }}

:   return info for debuff from self. e.g. `${Debuff[self].Slowed}`

### {{ renderMember(type='Debuff', name='Debuff[pet|warder]') }}

:   

### {{ renderMember(type='Debuff', name='Debuff', params='spell id ...') }}

:   return info for a specific debuff, or a list of debuffs. e.g. `${Debuff[5682].Slowed}` or for a list, `${Debuff[5682 2899 887].Slowed}`

<!--tlo-forms-end-->

## Associated DataTypes
<!--tlo-datatypes-start-->
## [`Debuff`](datatype-debuff.md)
{% include-markdown "projects/mq2debuffs/datatype-debuff.md" start="<!--dt-desc-start-->" end="<!--dt-desc-end-->" trailing-newlines=false %} {{ readMore('projects/mq2debuffs/datatype-debuff.md') }}
:    <h3>Members</h3>
    {% include-markdown "projects/mq2debuffs/datatype-debuff.md" start="<!--dt-members-start-->" end="<!--dt-members-end-->" %}
    {% include-markdown "projects/mq2debuffs/datatype-debuff.md" start="<!--dt-linkrefs-start-->" end="<!--dt-linkrefs-end-->" %}
    <!--tlo-datatypes-end-->

## Examples
<!--tlo-examples-start-->
HUD example,
```ini
[Elements]
PoisonCounter=1,400,170,0,250,50,${If[${Debuff.Poisoned},${Debuff.Poisoned} POISON,]}
DiseaseCounter=1,400,185,200,200,50,${If[${Debuff.Diseased},${Debuff.Diseased} DISEASE,]}
CurseCounter=1,400,200,250,200,150,${If[${Debuff.Cursed},${Debuff.Cursed} CURSE,]}
DrainHP=1,465,170,250,0,10,${If[${Debuff.HPDrain},-${Debuff.HPDrain} HP/tick,]}
DrainMana=1,465,185,0,50,250,${If[${Debuff.ManaDrain},-${Debuff.ManaDrain} Mana/tick ,]}
BadThings=1,400,220,255,0,10,${If[${Debuff.Snared},SNARED ,]}${If[${Debuff.Slowed},SLOWED ,]}${If[${Debuff.SpellSlowed},SPELLSLOWED ,]}${If[${Debuff.CastingLevel},EFFCASTLEVELDOWN ,]}${If[${Debuff.HealingEff},HEALEFFECTIVEDOWN ,]}${If[${Debuff.SpellDmgEff},SPELLDMGDOWN ,]}${If[${Debuff.ManaCost},MANACOSTUP ,]}
```
<!--tlo-examples-end-->

<!--tlo-linkrefs-start-->
[bool]: ../macroquest/reference/data-types/datatype-bool.md
[debuff]: datatype-debuff.md
<!--tlo-linkrefs-end-->