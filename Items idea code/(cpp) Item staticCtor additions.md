# Item.cpp staticCtor additions

Add these inside `Item::staticCtor()`.

These are skeletons.
You must replace:
- `TODO_ID_*`
- `IDS_ITEM_*`
- class choice where noted

```cpp
Item::prismarineShard =
    (new Item(TODO_ID_PRISMARINE_SHARD))
    ->setTextureName(L"prismarine_shard")
    ->setBaseItemTypeAndMaterial(eBaseItemType_treasure, eMaterial_magic)
    ->setDescriptionId(IDS_ITEM_PRISMARINE_SHARD);

Item::prismarineCrystals =
    (new Item(TODO_ID_PRISMARINE_CRYSTALS))
    ->setTextureName(L"prismarine_crystals")
    ->setBaseItemTypeAndMaterial(eBaseItemType_treasure, eMaterial_magic)
    ->setDescriptionId(IDS_ITEM_PRISMARINE_CRYSTALS);

Item::banner =
    (new Item(TODO_ID_BANNER)) // TODO choose subclass later if needed
    ->setTextureName(L"banner")
    ->setBaseItemTypeAndMaterial(eBaseItemType_HangingItem, eMaterial_cloth)
    ->setDescriptionId(IDS_ITEM_BANNER);

Item::endCrystal =
    (new Item(TODO_ID_END_CRYSTAL)) // TODO choose subclass later if needed
    ->setTextureName(L"end_crystal")
    ->setBaseItemTypeAndMaterial(eBaseItemType_treasure, eMaterial_glass)
    ->setDescriptionId(IDS_ITEM_END_CRYSTAL);

Item::elytra =
    (new Item(TODO_ID_ELYTRA)) // TODO choose subclass later if needed
    ->setTextureName(L"elytra")
    ->setBaseItemTypeAndMaterial(eBaseItemType_chestplate, eMaterial_cloth)
    ->setDescriptionId(IDS_ITEM_ELYTRA);

Item::chorusFruit =
    (new Item(TODO_ID_CHORUS_FRUIT)) // TODO choose subclass later if needed
    ->setTextureName(L"chorus_fruit")
    ->setBaseItemTypeAndMaterial(eBaseItemType_treasure, eMaterial_magic)
    ->setDescriptionId(IDS_ITEM_CHORUS_FRUIT);

Item::chorusFruitPopped =
    (new Item(TODO_ID_CHORUS_FRUIT_POPPED))
    ->setTextureName(L"chorus_fruit_popped")
    ->setBaseItemTypeAndMaterial(eBaseItemType_treasure, eMaterial_magic)
    ->setDescriptionId(IDS_ITEM_CHORUS_FRUIT_POPPED);

Item::beetrootSeeds =
    (new Item(TODO_ID_BEETROOT_SEEDS))
    ->setTextureName(L"beetroot_seeds")
    ->setBaseItemTypeAndMaterial(eBaseItemType_seed, eMaterial_carrot)
    ->setDescriptionId(IDS_ITEM_BEETROOT_SEEDS);

Item::beetroot =
    (new Item(TODO_ID_BEETROOT))
    ->setTextureName(L"beetroot")
    ->setBaseItemTypeAndMaterial(eBaseItemType_treasure, eMaterial_carrot)
    ->setDescriptionId(IDS_ITEM_BEETROOT);
```

## Notes
- In your codebase, the number inside `new Item(...)` is the real item ID minus 256.
- Safer first-pass items are:
  - prismarineShard
  - prismarineCrystals
  - chorusFruitPopped
  - beetrootSeeds
  - beetroot
