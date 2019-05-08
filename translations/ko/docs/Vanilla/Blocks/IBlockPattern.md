# IBlockPattern

An IBlockPattern is an interface that allows for combining several blocks into one object.  
It is comparable to what the [IIngredient](/Vanilla/Variable_Types/IIngredient/) Interface is to [IItemStacks](/Vanilla/Items/IItemStack/).

## 패키지 임포트하기

예를 들어 [Array](/AdvancedFunctions/Arrays_and_Loops/)를 캐스팅하려면 관련된 패키지를 임포트해야만 합니다. 안전을 위해서도 말입니다.   
`import crafttweaker.block.IBlockPattern;`

## IBlockDefinition 객체 호출

Technically, each time you call an [IBlock](/Vanilla/Blocks/IBlock/) object, you call an IBlockPattern object.  
But there are cases when you explicitly get an IBlockPattern Object as return.

* OR two [IBlocks](/Vanilla/Blocks/IBlock/)

## ZenGetters

| ZenGetter   | What does it do                                | Return Type                             |
| ----------- | ---------------------------------------------- | --------------------------------------- |
| blocks      | Lists all possible blocks for this object      | List<[IBlock](/Vanilla/Blocks/IBlock/)> |
| displayName | Returns the displayNames of the fitting blocks | String                                  |

## OR

You can OR two IBlockPattern Objects using the OR `|` Operator

## Matching

You can check if an IBlockPatternObject contains another using the `in` keyword.  
For example, you could check if a Block is in an IBlockPattern.