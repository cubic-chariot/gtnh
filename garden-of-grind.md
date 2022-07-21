GTNH: Garden of Grind
=====================

This document outlines a theoretical playthrough of the modpack
[GregTech: New Horizons](https://github.com/GTNewHorizons/GT-New-Horizons-Modpack),
in a skyblock-like setting.
We start from absolutely nothing,
and try to reconstruct as much as possible from GTNH.

I don't know much about GTNH itself,
so this document will evolve as I learn more about the modpack.


Rules
-----

Remove the mod Default World Generator
and create a superflat world with the preset `2;0;1;`.
This preset has Plains as the biome,
and no blocks at all.
You may not use the questbook rewards or travel to other dimensions.

Some structures may still generate, like Wichery circles;
you're not allowed to use them.
In the future,
this paragraph will be updated with instructions on how to disable them.


Prior Work
----------

- [Skyblock Ruleset by Order#0001](<https://docs.google.com/document/d/1Ajmpajbpw8H9rOpiPgX6AcUOcpdIfArwb-aoVrKly4I>);
    an earlier GTNH skyblock concept.
    The main differences is that we don't change game rules
    (most notably, we keep `gamerule doMobSpawning true`)
    and we start with no items.

- [Stone Age Thaum by Aura#0696](https://docs.google.com/document/d/1VF9HJPsaJasY_V_3OeJOX5RIRzGx5Xjfr-iBzzjfZGU);
    this documents outlines how to get started with Thaumcraft in Stone Age.


Getting Started
===============

The first thing that happens when you join the world described above is:
you fall in the void and die.
This creates an OpenBlocks grave with a block of dirt underneath.
When you respawn,
you will be on top of that block of dirt.
Throw yourself on the void again,
but a bit to the left.
This creates yet another block of dirt.
Repeat a few hundred times to gather building blocks.
Then we progress as follows:

- Build a rudimentary mobfarm.
    Kill enough infernal mobs until one of them drops a golden apple.

- Get a villager. Here's how:
    Get a witch and a zombie villager to spawn close to one another,
    anger the witch so that she throws a weakness potion at you,
    be close enough to the zombie so that it gets hit too,
    and feed it the golden apple;
    a few minutes later, you have a villager!

- Convert a few more villagers.
    Botania makes them shed emeralds,
    so you can purchase a Pam's sapling from a farmer.
    (Even without shedding,
    Cleric villagers trade rotten flesh for emeralds,
    and you just need one emerald to get a sapling.)
    This gives access to wood.

- The crafting table recipe was unfortunately Gregified.
    Go back to your mob farm and wait till a Gravel Creeper spawns;
    it explodes in a bunch of gravel,
    which can be crafted into flint,
    which gives us crafting tables.
    (You can also make chests now,
    but flint is probably too precious for now,
    so use the droppers/dispensers dropped by infernal mobs as makeshift storage.)

- Go back to your mob farm and wait till a drowning creeper appears.
    Let it explode.
    This generates water and some cobblestone.
    Unfortunately,
    you probably don't have a pickaxe yet,
    and GTNH disables most non-Tinker's Construct pickaxes;
    therefore you must "mine" that cobblestone with creepers.
    With the flint you saved from before,
    you can craft a furnace.
    This gives us stone and thus mortars.

- Zombies drop iron ingots, which can be used to make buckets and a full set of Gregtech tools.
    They also drop potatoes and carrots,
    which allows us to get started with crops!
    (Infernal mobs sometimes drop hoes.)
    Aim for the oreberries.
    Infernal mobs also rarely drop diamonds,
    so you can make a plant lens (buy glass from a librarian villager).

- The mortar can be used to grind wood blocks to woodpulp,
    which gives us papers and TiCon's Blank Pattern.
    With some string you can craft the basic TiCon crafting stations
    (stencil table, part builder, tool station),
    giving access to Tinker's tools with flint heads!
    Also make a brick wooden form.

- The Tinker's Construct oreberries you bred a few steps before
    don't need the corresponding block underneath to drop their resource.
    Use the mortar to get tiny dusts
    and smelt them in furnace to get ingots.
    Mixing tin and copper in a crafting table gives us access to bronze.

- Build a Railcraft Iron Tank.
    The walls only need iron,
    and the valve needs bronze.
    Place a valve on top of the tank,
    craft an XP drain,
    and place it over the valve.
    Congratulations, now you have access to XP buckets!

- Get clay dust from XP buckets,
    transform it into clay balls and then to unfired clay bricks,
    and smelt and assemble them into brick blocks.
    Together with the bronze,
    this gives us much of steam age:
    small coal boiler,
    steam alloy smelter,
    steam compressor (infernal mobs drop pistons),
    steam extractor,
    steam macerator,
    steam forge hammers (as the compressor gives us iron blocks).
    The Railcraft Water Tank is doable here as well.

- Forge hammers can hammer the drowning creeper's cobblestone down to gravel and sand.
    So we can make unfired coke oven bricks
    and assemble coke ovens;
    this gives us access to charcoal and thus torches!
    With XP buckets this allows us to make and use a Bricked Blast Furnace.

- Crop breeding gives stickreed which gives raw rubber dust.
    XP buckets gives sulfur.
    Since we have a steam alloy smelter,
    we get access to rubber.

- You probably got some weeds during crop breeding.
    If they are left to mature,
    they will transform nearby farmland into grass blocks.
    Let the grass spread;
    this allows passive mobs to spawn.

- Librarian villagers sell bookshelves,
    Heretic villagers sell profane wands,
    and a Thaumcraft table can be made using only iron and wood.
    Witches drop glass bottles,
    you got rubber a few steps above,
    chickens gives feathers,
    and crops gives us ink sacs;
    thus we can craft scribing tools.
    This allows us to get started with Thaumcraft.


Possibly Unsurmountable Obstacles
=================================

Although the profane wand gives us a head start in Thaumcraft without greatwood and silverwood,
we eventually will want to craft higher-tier wands,
and there are other things that require them.
Unfortunately I don't know how to get them in this context.

Several things beyond MV needs lenses,
including HV circuits and Thaumcraft's runic matrix.
Unfortunately,
we have no access to flawless or exquisite gems
(as the implosion compressor is gated behind HV circuits),
so the only way of getting e.g. green sapphire lenses
is by using an MV lathe with green sapphire plates.
But the MV lathe itself requires a flawless diamond.
