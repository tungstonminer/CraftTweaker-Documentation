# MCBlockDisplayReader

One of [MCWorld](/vanilla/api/world/MCWorld)'s supertype, used for display calculation.

## Importing the class

It might be required for you to import the package if you encounter any issues (like casting an Array), so better be safe than sorry and add the import at the very top of the file.
```zenscript
import crafttweaker.api.world.MCBlockDisplayReader;
```


## Methods

:::group{name=canSeeSky}

Gets if can see sky at a given position

Return Type: boolean

```zenscript
// MCBlockDisplayReader.canSeeSky(pos as BlockPos) as boolean

myMCBlockDisplayReader.canSeeSky(new BlockPos(0, 1, 2));
```

| Parameter | Type | Description |
|-----------|------|-------------|
| pos | [BlockPos](/vanilla/api/util/BlockPos) | The position to look up. |


:::

:::group{name=getBlockState}

Gets the block state at a given position.

Return Type: [MCBlockState](/vanilla/api/block/MCBlockState)

```zenscript
// MCBlockDisplayReader.getBlockState(pos as BlockPos) as MCBlockState

myMCBlockDisplayReader.getBlockState(new BlockPos(0, 1, 2));
```

| Parameter | Type | Description |
|-----------|------|-------------|
| pos | [BlockPos](/vanilla/api/util/BlockPos) | The position to look up. |


:::

:::group{name=getLightValue}

Gets the light level at a given position

Return Type: int

```zenscript
// MCBlockDisplayReader.getLightValue(pos as BlockPos) as int

myMCBlockDisplayReader.getLightValue(new BlockPos(0, 1, 2));
```

| Parameter | Type | Description |
|-----------|------|-------------|
| pos | [BlockPos](/vanilla/api/util/BlockPos) | The position to look up. |


:::

:::group{name=getTileEntity}

Gets the tile entity at a given position.

Return Type: [MCTileEntity](/vanilla/api/tileentity/MCTileEntity)?

```zenscript
// MCBlockDisplayReader.getTileEntity(pos as BlockPos) as MCTileEntity?

myMCBlockDisplayReader.getTileEntity(new BlockPos(0, 1, 2));
```

| Parameter | Type | Description |
|-----------|------|-------------|
| pos | [BlockPos](/vanilla/api/util/BlockPos) | The position of the tile entity. |


:::


