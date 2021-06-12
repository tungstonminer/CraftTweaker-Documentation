# Survivalist

## Chopping Block

### InputStack, OutputStack, {outputMultiplier}, {hitCountMultiplier}

```zenscript
gigaherz.survivalist.Choppable.addRecipe(IIngredient input,  IItemStack output, outputMultiplier, hitCountMultiplier);
```

##### 例子

```zenscript
gigaherz.survivalist.Choppable.addRecipe(<minecraft:bone>,<minecraft:dye:15>, 1.0, 1.0);
```

### OutputStack, {InputStack}

```zenscript
gigaherz.survivalist.Choppable.removeRecipe(IIngredient output, IIngredient input);
```

##### 例子

```zenscript
gigaherz.survivalist.Choppable.removeRecipe(<minecraft:stick>);
```

## Drying Rack

### InputStack, OutputStack, Time in Ticks

```zenscript
gigaherz.survivalist.Dryable.addRecipe(IIngredient input, IItemStack output, int time);
```

##### 例子

```zenscript
gigaherz.survivalist.Dryable.addRecipe(<minecraft:rotten_flesh>, <minecraft:leather>, 300);
```

### OutputStack, {InputStack}

```zenscript
gigaherz.survivalist.Dryable.removeRecipe(IIngredient output, IIngredient input);
```

##### 例子

```zenscript
gigaherz.survivalist.Dryable.removeRecipe(<minecraft:leather>, <minecraft:rotten_flesh>);
```

#### InputStack can be ore dictionary and anything surrounded by {} is optional