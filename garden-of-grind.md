GTNH: Garden of Grind
=====================

This document outlines a playthrough of the modpack
[GregTech: New Horizons](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack),
in a skyblock-like setting.
We start from absolutely nothing,
and try to reconstruct as much as possible from GTNH.

I don't know much about GTNH itself,
so this document will evolve as I learn more about the modpack.
In particular,
it is lacking bees, Botania and a good chunk of Thaumcraft.


Rules
-----

Remove the mod Default World Generator
and create a superflat world with the preset `2;0;1;`.
This preset has Plains as the biome,
and no blocks at all.
You may not use the questbook rewards or travel to other dimensions.

Change the following configs in `witchery.cfg`:
```
    B:GenerateApothecaries=false
    B:GenerateBookShops=false
    B:GenerateCovens=false
    B:GenerateHobgoblinHuts=false
    B:GenerateShacks=false
    B:GenerateWickerMen=false
    B:GenerateWitchHuts=false
```

Change the following configs in `Thaumcraft.cfg`:
```
    B:generate_aura_nodes=false
    B:generate_structures=false
```

You may cheat in the following items:
- One greatwood sapling and one silverwood sapling after crafting a runic matrix.
- A single flawless diamond after you build your first MV machine casing.

The reason is because I don't know how to get these items without cheating them in.
[This is discussed below](#possibly-unsurmountable-obstacles).


### Alternatives

- Use the questbook instead of cheating in items.
    This gives access to the magical saplings,
    diamond ores,
    and some bees.

### Sanity-preserving concessions

- Make the superflat preset be `2;0;68;`.
    This changes the biome to Grasslands,
    which is much better for IC2 crops than plains.

- Cheat in one acacia sapling once you convert your first villager.

- Use shaders to cheese hardcore darkness,
    or configure `HardcoreDarkness.cfg > S:"Dimension Blacklist"` to be `0`.

External Links
--------------

- [Garden of Grind by Order#0001](<https://docs.google.com/document/d/1g4EcDbfhZtiyqIE2WPkSiKTwP4MbNpiFT_o_agkPGgk/edit>);
    a detailed description of our Garden of Grind run.
    We used the questbook and grasslands alternatives.

- [Skyblock Ruleset by Order#0001](<https://docs.google.com/document/d/1Ajmpajbpw8H9rOpiPgX6AcUOcpdIfArwb-aoVrKly4I>);
    an earlier GTNH skyblock concept.
    The main differences is that we don't change game rules
    (most notably, we keep `gamerule doMobSpawning true`)
    and we start with no items.

- [Stone Age Thaum by Aura#0696](https://docs.google.com/document/d/1VF9HJPsaJasY_V_3OeJOX5RIRzGx5Xjfr-iBzzjfZGU);
    this documents outlines how to get started with Thaumcraft in Stone Age.


The Route
=========

- [Getting started](gog-getting-started.md)
    documents from the very beginning till LV.

- [Between LV and MV](gog-lv-mv.md)
    we establish several important resource-gathering methods
    and hit the flawless diamond roadblock.
    At this point,
    you either cheat in a flawless diamond,
    or get one by sifting diamond ores from the questbook.


Possibly Unsurmountable Obstacles
=================================

Greatwood and Silverwood
------------------------

Although the profane wand gives us a head start in Thaumcraft without greatwood and silverwood,
we eventually will want to craft higher-tier wands,
and there are other things that require them.
Unfortunately I don't know how to get them in this context;
besides worldgen and the questbook,
I think that all methods of obtaining these saplings
require them to begin with.
