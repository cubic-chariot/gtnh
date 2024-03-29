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

You may cheat in a single flawless diamond after you build your first MV machine casing.
The reason is because I don't know how to get one without cheating them in.
[This is discussed here](gog-lv-mv.md#the-lens-obstacle).

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
    - Alternatively,
        you can savescum the first trades of the first villager.
        In Minecraft 1.8 and below,
        zombie villagers don't have a profession,
        which is rerolled once the zombie is cured.

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

The following pages outline the several steps of the run.
Practicality is _not_ the focus of the outline below;
for this, see e.g. [our run here](<https://docs.google.com/document/d/1g4EcDbfhZtiyqIE2WPkSiKTwP4MbNpiFT_o_agkPGgk/edit>).

- [Getting started](gog-getting-started.md)
    documents from the very beginning till LV.

- [Between LV and MV](gog-lv-mv.md)
    we establish several important resource-gathering methods
    and hit the flawless diamond roadblock.
    At this point,
    you either cheat in a flawless diamond,
    or get one by sifting diamond ores from the questbook.

- [Between late MV and EV](gog-mv-ev.md)
    we have to do some tierskipping to get titanium,
    and we get close to running out of resources that can be obtained from crops.
