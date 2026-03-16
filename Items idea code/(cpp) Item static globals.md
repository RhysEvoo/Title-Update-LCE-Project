# Item.cpp static global definitions

Add these near the other `Item *Item::... = NULL;` lines:

```cpp
Item *Item::prismarineShard = NULL;
Item *Item::prismarineCrystals = NULL;
Item *Item::banner = NULL;
Item *Item::endCrystal = NULL;
Item *Item::elytra = NULL;
Item *Item::chorusFruit = NULL;
Item *Item::chorusFruitPopped = NULL;
Item *Item::beetrootSeeds = NULL;
Item *Item::beetroot = NULL;
```
