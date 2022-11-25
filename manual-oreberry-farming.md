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
