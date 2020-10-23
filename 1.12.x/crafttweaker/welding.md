Welding recipe manager has three methods for recipe manipulation:

```zenscript
// Import welding methods into your script
import mods.terrafirmacraft.Welding;
// Adds a recipe with the given parameters
Welding.addRecipe(String registryName, IIngredient input1, IIngredient input2, IItemStack output, int minTier);
// Removes all recipes that produce a given output
Welding.removeRecipe(IItemStack output);
// Removes a single recipe by registry name
Welding.removeRecipe(String registryName);
```

As with anvil recipes, the same rules for input applies here. The input must be forgeable(see [ItemRegistry](ItemRegistry) for registering forging capability to an item) and can't be stacked.