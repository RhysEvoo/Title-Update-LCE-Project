# Recipes.cpp examples

These are only examples.
Do not add all of them unless the behavior matches the version you want.

```cpp
// Prismarine Crystals from shards - example only
addShapelessRecipy(new ItemInstance(Item::prismarineCrystals, 1),
    new ItemInstance(Item::prismarineShard, 1),
    new ItemInstance(Item::prismarineShard, 1),
    new ItemInstance(Item::prismarineShard, 1),
    new ItemInstance(Item::prismarineShard, 1),
    L'S');

// Banner - example pattern, adjust if your branch expects a banner subclass/item
addShapedRecipy(new ItemInstance(Item::banner, 1),
    L"sssctcig",
    L"###",
    L"###",
    L" X ",
    L'#', Tile::cloth, L'X', Item::stick,
    L'S');
```

## Notes
- `beetrootSeeds` and `chorusFruit` are usually found/generated rather than crafted in many versions.
- `elytra` and `endCrystal` often need custom behavior and may not be simple crafting-only items.
