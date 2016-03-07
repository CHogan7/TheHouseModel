# TheHouseModel
- Tile: An object with the responsibiliy of tracking unallocated items, current entity occupying the tile, the ability to pass over or through the tile, the tile biome, and the tile type.
- Room: A room inherently has a biome which determines its graphics. It also has a type corresponding to how the room is laid out. It tracks where the entrance to the room is, and the exit to the room. It also has a label of the room number showing where you are at the current moment in terms of the entire map.
- Entity: An entity is an object which can interact with other objects in the world. It inherently has many properties and keeps track of its to determine the location of other entities.
- Item: An abstract of an object that is identified through ennumeration, has a name, and tracks its use.
  - HealItem: An item that restores health, and increases in efficiacy determined by the strength property.
  - ExpItem: An item gives you a flat amount of experience that contributes to your total level. Effecitveness is determined elsewhere.
- PlaceHolderItem: This object is representative of the lack of an item.

- Equip[RENOAINFAOIWNDOAIWNDOIWANDWAOIDNAWODIANWDOWAINDAOWDNIWANDOAWIDNWAD]: An object that modifies several entity modifiers, which affect its ability to perform combat.

Ennumerated Types and Purposes:
- tileType {WALL, FLOOR, DOOR}: The value that determines if a specific tile is a wall, a floor, or a door, to help identify properties later on.
- tileBiome {FOREST, MOUNTAIN, CAVERN, URBAN, FINAL}: The value that determines the images used in a specific area with a certain type of look in mind.
- roomType {bottomLeft,	bottomTop, bottomRight,	leftTop,	leftRight,	leftBottom,	topRight,	topBottom,	topLeft,	rightBottom,rightLeft,	rightTop}: Determines the locations of the door in the order of door entrance and door exit.
- itemType {WEAPON,	ARMOR,	ACCESSORY,	HEAL,	EXP,	PLACEHOLDER}: Determines the properties of the items that one can acquire throughout the game.
- Size {SMALL, MEDIUM, LARGE}: Determines the efficiacy of a consumable item.
- Direction {NORTH, SOUTH, EAST, WEST}: Determines the orientation of an entity.
