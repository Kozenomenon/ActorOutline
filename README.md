# ActorOutline
Ark Survival Evolved Mod Assets for adding a custom stencil outline to a target actor. Such as a dino.
![ActorOutline_Example](/Images/ActorOutline_Example.png)
![Multi Target Example](/Images/Multi_Target_Stencil.png)

## Setup / Use in PIE
1. Download the source
2. Place the `ActorOutline` folder in your kit's `/Mods` folder (file explorer, outside the kit)
3. Path in kit to assets listed below should be: `/Game/Mods/ActorOutline`
4. Open `TestMapArea_ActorOutline` 
5. Click PIE button
6. Spawn Dinos & Structures
7. Toggle between Single/Multi stencils using `[N]` (Weapon Accessory)
8. Toggle buff targeting on/off using `[RMB]` (Targeting / Iron Sights)

## Assets
- **/MultiTargetStencil/Buff_ActorOutline_Multi**
  - *Player buff that manages the multi-target stencil.*
  - *Setup to stencil multiple targets within range of player.*
  - *Buff Defaults apply to Stencil Material dynamically.*
- **/MultiTargetStencil/PP_ActorOutline_Multi**
  - *Base Stencil material with all the visual logic.*
- **/MultiTargetStencil/PP_ActorOutline_Multi_MIC**
  - *Material instance referenced by the buff (and your PGD).*
- **/SingleTargetStencil/Buff_ActorOutline_Single**
  - *Player buff that manages the single target stencil.*
  - *Setup to stencil whatever the player is looking at.*
  - *Changed this from what the example did before, left old logic disconnected in BuffClientTick.* 
  - *Now can use any color - thanks Legendarsreign & HexenLord* 
  - *Buff Defaults apply to Stencil Material dynamically.*
- **/SingleTargetStencil/PP_ActorOutline_Single**
  - *Base Stencil material with all the visual logic.*
- **/SingleTargetStencil/PP_ActorOutline_Single_MIC**
  - *Material instance referenced by the buff (and your PGD).*
  
## PIE Things
- **ActorOutline_CCA**
  - *Used so buff applies to player right away in PIE.*
  - *Template used from: [ArkTemplates Open Source](https://github.com/Kozenomenon/ArkTemplates)*
- **PrimalGameData_BP_ActorOutline** 
  - *Test Harness to run the example in PIE.* 
  - *PP MIC in AdditionalBuffPostProcessEffects array.* 
  - *Buff in AdditionalDefaultBuffs array.* 
  - *CCA in Singletons array.* 
- **TestMapArea_ActorOutline** 
  - *Test map to run the example in PIE.* 
