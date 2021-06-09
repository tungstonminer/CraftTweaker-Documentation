# BracketHandlers

I advise against using the static methods in this class directly as they may be merged into CrT's BEP at any point. If you need to access the Bracket Expression Parser methods dynamically, you can use
 ```zencode
 var myName = "misc";
 <itemgroup:${myName}>
 ```

This class was added by a mod with mod-id `contenttweaker`. Так что если вы хотите использовать эту функцию, вам нужно установить этот мод.

## Импорт класса

It might be required for you to import the package if you encounter any issues (like casting an Array), so better be safe than sorry and add the import at the very top of the file.
```zenscript
import mods.contenttweaker.BracketHandlers;
```


## Static Methods

:::group{name=getCoTBlock}

Gets the registered advanced CoT block. Will throw an error if the block could not be found

Returns: The found IIsCotBlock  
Return Type: [CoTBlockAdvanced](/mods/contenttweaker/API/block/advance/CoTBlockAdvanced)

```zenscript
<advancedblock:test_block>

// BracketHandlers.getCoTBlock(tokens as string) as CoTBlockAdvanced

BracketHandlers.getCoTBlock("test_block");
```

| Параметр | Тип    | Description                                       |
| -------- | ------ | ------------------------------------------------- |
| tokens   | string | What you would createDataCompound in the BEP call |


:::

:::group{name=getCoTItem}

Gets the registered advanced CoT item. Will throw an error if the item could not be found

Returns: The found IIsCotItem  
Return Type: [CoTItemAdvanced](/mods/contenttweaker/API/item/advance/CoTItemAdvanced)

```zenscript
<advanceditem:test_item>

// BracketHandlers.getCoTItem(tokens as string) as CoTItemAdvanced

BracketHandlers.getCoTItem("test_item");
```

| Параметр | Тип    | Description                                       |
| -------- | ------ | ------------------------------------------------- |
| tokens   | string | What you would createDataCompound in the BEP call |


:::

:::group{name=getItemGroup}

Gets the itemGroup. Will throw an error if the group could not be found

Returns: The found MCItemGroup  
Return Type: [MCItemGroup](/mods/contenttweaker/API/item/MCItemGroup)

```zenscript
<itemgroup:misc>

// BracketHandlers.getItemGroup(tokens as string) as MCItemGroup

BracketHandlers.getItemGroup("misc");
```

| Параметр | Тип    | Description                                 |
| -------- | ------ | ------------------------------------------- |
| tokens   | string | What you createDataCompound in the BEP call |


:::
