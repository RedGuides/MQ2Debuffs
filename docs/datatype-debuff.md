---
tags:
  - datatype
---
# `Debuff`

<!--dt-desc-start-->
Reports harmful effects, number of curse/disease/poison counters and various other detriments.
<!--dt-desc-end-->

## Members
<!--dt-members-start-->
### {{ renderMember(type='int', name='Poisoned') }}

:   *#* of poison counters on you

### {{ renderMember(type='int', name='Diseased') }}

:   *#* of disease counters on you

### {{ renderMember(type='int', name='Cursed') }}

:   *#* of curse counters on you

### {{ renderMember(type='int', name='Corrupted') }}

:   *#* of corruption counters on you

### {{ renderMember(type='int', name='Poisons') }}

:   *#* of poison spells affecting you

### {{ renderMember(type='int', name='Diseases') }}

:   *#* of disease spells affecting you

### {{ renderMember(type='int', name='Curses') }}

:   *#* of curse spells affecting you

### {{ renderMember(type='int', name='Corruptions') }}

:   *#* of corruption spells affecting you

### {{ renderMember(type='int', name='Count') }}

:   *#* of debuffs that need cured, does not include snare

### {{ renderMember(type='int', name='HPDrain', params='ѕtring') }}

:   * No index= Amount of HP you are losing per tick from debuffs. This value is POSITIVE
* string= Disease, Poison, Curse, All: Number of specific counters effecting HP

### {{ renderMember(type='int', name='ManaDrain', params='ѕtring') }}

:   * No index= Amount of Mana you are losing per tick from debuffs. This value is POSITIVE
* string= Disease, Poison, Curse, All: Number of specific counters effecting Mana

### {{ renderMember(type='int', name='EnduranceDrain', params='ѕtring') }}

:   * No index= Amount of Endurance you are losing per tick from debuffs. This value is POSITIVE
* string= Disease, Poison, Curse, All: Number of specific counters effecting Endurance

### {{ renderMember(type='bool', name='Slowed') }}

:   True if you are Slowed (melee attacks), False if not

### {{ renderMember(type='bool', name='SpellSlowed') }}

:   True if you are SpellSlowed (spell haste reduction), False if not

### {{ renderMember(type='bool', name='Snared') }}

:   True if your are Snared, False if not

### {{ renderMember(type='bool', name='ManaCost') }}

:   True if your Spell Mana Cost has been raised, False if not

### {{ renderMember(type='bool', name='CastingLevel') }}

:   True if your Effective Casting Level has been reduced, False if not

### {{ renderMember(type='bool', name='HealingEff') }}

:   True if your Healing Effectiveness has been reduced, False if not

### {{ renderMember(type='bool', name='SpellDmgEff') }}

:   True if your Spell Damage Effectiveness has been reduced, False if not

### {{ renderMember(type='bool', name='Blind') }}

:   True if you are blind

### {{ renderMember(type='bool', name='Charmed') }}

:   True if you are charmed

### {{ renderMember(type='bool', name='Feared') }}

:   True if you are feared

### {{ renderMember(type='bool', name='Silenced') }}

:   True if you are silenced

### {{ renderMember(type='bool', name='Invulnerable') }}

:   True if you are invulnerable

### {{ renderMember(type='bool', name='Detrimentals') }}

:   True if you have any detrimental effects on you

### {{ renderMember(type='int', name='Counters') }}

:   *#* of poison/disease/curse/corruption counters on yourself

### {{ renderMember(type='bool', name='Rooted') }}

:   True if you are rooted

<!--dt-members-end-->

<!--dt-linkrefs-start-->
[bool]: ../macroquest/reference/data-types/datatype-bool.md
[int]: ../macroquest/reference/data-types/datatype-int.md
<!--dt-linkrefs-end-->
