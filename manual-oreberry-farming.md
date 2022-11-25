Efficient Manual Oreberry Farming
=================================

This article describes an efficient way of manually farming oreberries planted on IC2 cropsticks.
The method described here is by no means competitive with automatic farming
and should only be used if Gregtech's Crop Manager is inaccessible
(e.g. in [skyblock](./garden-of-grind.md)).


Background
----------

Tinker's Construct adds six types of oreberry
(iron oreberry, gold oreberry, copper oreberry, tin oreberry, aluminum oreberry,
and concentrated essence berry;
the latter is still considered an oreberry even though its not named as such).
Although the oreberry bushes are not accessible in GTNH,
the oreberries themselves are,
and they can be planted on Industrial Craft 2's cropsticks.

Oreberries have 4 growth stages.
They only grow if the light level is `<= 10`.
They can be harvested on the 3rd stage to get 2 oreberry items of the respective type,
and on the 4th stage to get 6.
However they need a block of their respective metal to reach the 4th stage.
(The exception is the essence berry,
which grows in sunlight despite the tooltip,
needs skeleton skulls underneath to drop 6 berries,
and reaches the 4th stage even without skeleton skulls underneath.)


Problem Statement
-----------------

The goal is to make the process of manually farming oreberries as efficient as possible.
"Efficient" means the player should spend as little as possible walking in the farm.

The main obstacle is that,
when the oreberry is harvested (right-clicked),
the oreberry item flies to a random direction.
The design below minimizes backtracking to grab the items that fly away from the player.


The Design
----------

The top-down layout of the farm is the following:

    ....................
    .FFFFFFFFFFFFFFFFFF.
    .FFFFFFFFFFFFFFFFFF.
    .....:........:.....
    .FFFFWFFFFFFFFWFFFF.
    .FFFFWFFFFFFFFWFFFF.
    .....:........:.....
    .FFFFFFFFFFFFFFFFFF.
    .FFFFFFFFFFFFFFFFFF.
    ....................

    . = empty space
    : = vanilla sign
    F = farmland with a cropstick on top
    W = water source block with a solid block on top

This layout essentially alternates between two rows of farmland (with oreberries)
and one row with empty space,
with some optimizations to account for the need for water hydrating the farmland.
This layout can be tiled horizontally and vertically;
only two empty columns may exist,
but there must be an empty row between every two rows of farmland.

### Harvest procedure

It is possible to minimize backtracking by interweaving harvest and gathering phases,
as described below.

    Row 0: empty
    Row 1: farmland
    Row 2: farmland
    Row 3: empty
    Row 4: farmland
    Row 5: farmland
    Row 6: empty
    Row 7: farmland
    Row 8: farmland
    Row 9: empty

(Water and signs are irrelevant here.)

1. Enter empty row 0.
    Face farmland row 1,
    hold right-click, and traverse row 0 without stopping.
    This will harvest all the oreberries in row 1,
    but it will leave some items behind.
    Do _not_ backtrack to pick them up.
    This is a "**harvest phase**".

2. Enter empty row 3. Face farmland row 2 and traverse row 3,
    performing a harvest phase on row 2.
    (We are setting up the repeating pattern;
    this is the only time two harvest phases happens in a row.)

3. Enter empty row 0.
    Touch the farmland in row 1 with your character,
    and traverse row 0.
    This is a "**gathering phase**".
    This will collect all of the leftover items in farmland row 1.

4. Enter empty row 3.
    We will perform a "combined **harvest-gathering phase**" now.
    Face farmland row 4,
    and touch farmland row 2 with the back of your character.
    Holding right-click,
    traverse empty row 3 whilst still touching farmland row 2.
    This will harvest all oreberries in farmland row 4,
    leaving some behind,
    and also gather all items in farmland row 2.
    Now all oreberries in farmland rows 1 and 2 are harvested
    and all of its items are collected.

5. Repeat steps 2-4 three rows further;
    i.e. perform a harvest phase on farmland row 5 traversing empty row 6,
    perform a gathering phase on farmland row 4 traversing empty row 3,
    and perform a combined harvest phase on farmland row 7
    and gathering phase on farmland row 5 traversing empty row 6.

6. In general,
    you will perform a harvest phase on farmland row `3n-1` traversing empty row `3n`,
    perform a gathering phase on farmland row `3n-2` traversing empty row `3n-3`,
    and perform a combined harvest phase on farmland row `3n+1`
    and gathering phase on farmland row `3n-1` traversing empty row `3n`.

7. Finally,
    perform a harvest phase in the last farmland row traversing the last empty row
    (rows 8 and 9 in the diagram above),
    and perform a gathering phase on each of the last two farmland rows
    (rows 7 and 8 in the diagram above).

In the end,
the first and last empty rows will be traversed twice,
and the other empty rows will be traversed 3 times.
Thus tiling the layout vertically increases its efficiency,
reducing the number of traversals proportional to the number of farmland rows,
asymptotically approaching 1.5 empty row traversals per farmland row.
