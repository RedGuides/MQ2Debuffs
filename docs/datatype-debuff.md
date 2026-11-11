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
/// member | int Poisoned
*#* of poison counters on you
///

/// member | int Diseased
*#* of disease counters on you
///

/// member | int Cursed
*#* of curse counters on you
///

/// member | int Corrupted
*#* of corruption counters on you
///

/// member | int Poisons
*#* of poison spells affecting you
///

/// member | int Diseases
*#* of disease spells affecting you
///

/// member | int Curses
*#* of curse spells affecting you
///

/// member | int Corruptions
*#* of corruption spells affecting you
///

/// member | int Count
*#* of debuffs that need cured, does not include snare
///

/// member | int HPDrain[string]
* No index= Amount of HP you are losing per tick from debuffs. This value is POSITIVE
* string= Disease, Poison, Curse, All: Number of specific counters effecting HP
///

/// member | int ManaDrain[string]
* No index= Amount of Mana you are losing per tick from debuffs. This value is POSITIVE
* string= Disease, Poison, Curse, All: Number of specific counters effecting Mana
///

/// member | int EnduranceDrain[string]
* No index= Amount of Endurance you are losing per tick from debuffs. This value is POSITIVE
* string= Disease, Poison, Curse, All: Number of specific counters effecting Endurance
///

/// member | bool Slowed
True if you are Slowed (melee attacks), False if not
///

/// member | bool SpellSlowed
True if you are SpellSlowed (spell haste reduction), False if not
///

/// member | bool Snared
True if your are Snared, False if not
///

/// member | bool ManaCost
True if your Spell Mana Cost has been raised, False if not
///

/// member | bool CastingLevel
True if your Effective Casting Level has been reduced, False if not
///

/// member | bool HealingEff
True if your Healing Effectiveness has been reduced, False if not
///

/// member | bool SpellDmgEff
True if your Spell Damage Effectiveness has been reduced, False if not
///

/// member | bool Blind
True if you are blind
///

/// member | bool Charmed
True if you are charmed
///

/// member | bool Feared
True if you are feared
///

/// member | bool Silenced
True if you are silenced
///

/// member | bool Invulnerable
True if you are invulnerable
///

/// member | bool Detrimentals
True if you have any detrimental effects on you
///

/// member | int Counters
*#* of poison/disease/curse/corruption counters on yourself
///

/// member | bool Rooted
True if you are rooted
///

<!--dt-members-end-->

<!--dt-linkrefs-start-->
[bool]: ../macroquest/reference/data-types/datatype-bool.md
[int]: ../macroquest/reference/data-types/datatype-int.md
<!--dt-linkrefs-end-->
