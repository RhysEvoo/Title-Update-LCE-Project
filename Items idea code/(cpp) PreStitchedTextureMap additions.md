# PreStitchedTextureMap.cpp additions

Add these inside the non-terrain branch of `loadUVs()`.

Replace `X` and `Y` with the real grid coordinates from `items.png`.

```cpp
texturesByName.insert(stringIconMap::value_type(
    L"prismarine_shard",
    new SimpleIcon(L"prismarine_shard", slotSize*X, slotSize*Y, slotSize*(X+1), slotSize*(Y+1))
));

texturesByName.insert(stringIconMap::value_type(
    L"prismarine_crystals",
    new SimpleIcon(L"prismarine_crystals", slotSize*X, slotSize*Y, slotSize*(X+1), slotSize*(Y+1))
));

texturesByName.insert(stringIconMap::value_type(
    L"banner",
    new SimpleIcon(L"banner", slotSize*X, slotSize*Y, slotSize*(X+1), slotSize*(Y+1))
));

texturesByName.insert(stringIconMap::value_type(
    L"end_crystal",
    new SimpleIcon(L"end_crystal", slotSize*X, slotSize*Y, slotSize*(X+1), slotSize*(Y+1))
));

texturesByName.insert(stringIconMap::value_type(
    L"elytra",
    new SimpleIcon(L"elytra", slotSize*X, slotSize*Y, slotSize*(X+1), slotSize*(Y+1))
));

texturesByName.insert(stringIconMap::value_type(
    L"chorus_fruit",
    new SimpleIcon(L"chorus_fruit", slotSize*X, slotSize*Y, slotSize*(X+1), slotSize*(Y+1))
));

texturesByName.insert(stringIconMap::value_type(
    L"chorus_fruit_popped",
    new SimpleIcon(L"chorus_fruit_popped", slotSize*X, slotSize*Y, slotSize*(X+1), slotSize*(Y+1))
));

texturesByName.insert(stringIconMap::value_type(
    L"beetroot_seeds",
    new SimpleIcon(L"beetroot_seeds", slotSize*X, slotSize*Y, slotSize*(X+1), slotSize*(Y+1))
));

texturesByName.insert(stringIconMap::value_type(
    L"beetroot",
    new SimpleIcon(L"beetroot", slotSize*X, slotSize*Y, slotSize*(X+1), slotSize*(Y+1))
));
```

## Notes
- The icon name must exactly match the name used in `setTextureName(...)`.
- `slotSize` in your source is `1.0f / 16.0f`, so the coordinates are grid slots, not pixel values.
